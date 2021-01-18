> # Class 13 *Jan 19 2021:*

> ## Topics

  1. Local Storage [Referance](http://diveinto.html5doctor.com/storage.html)
  
---

#### THE PAST, PRESENT & FUTURE OF LOCAL STORAGE FOR WEB APPLICATIONS:

* **The read-only localStorage property allows you to access a Storage object for the Document's origin; the stored data is saved across browser sessions. localStorage is similar to sessionStorage, except that while data stored in localStorage has no expiration time, data stored in sessionStorage gets cleared when the page session ends — that is, when the page is closed**


#### Using HTML5 Storage:

**From your JavaScript code, you’ll access HTML5 Storage through the localStorage object on the global window object. Before you can use it, you should detect whether the browser supports it.**

        function supports_html5_storage() {
        try {
            return 'localStorage' in window && window['localStorage'] !== null;
        } catch (e) {
            return false;
        }
        }


**Or by Using Modernizer:**

        if (Modernizr.localstorage) {
            // window.localStorage is available!
            } else {
            // no native support for HTML5 storage :(
            // maybe try dojox.storage or a third-party solution
            }


* **HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key.**

    1. The named key is a string. 
    
    2. The data can be any type supported by JavaScript including strings, Booleans, integers, or floats. 

        interface Storage {
            getter any getItem(in DOMString key);
            setter creator void setItem(in DOMString key, in any data);
            };

**Example:**

        var foo = localStorage.getItem("bar");
        // ...
        localStorage.setItem("bar", foo);
        …could be rewritten to use square bracket syntax instead:

        var foo = localStorage["bar"];
        // ...
        localStorage["bar"] = foo;

* **methods for removing the value for a given named key, and clearing the entire storage area (that is, deleting all the keys and values at once).**

        interface Storage {
        deleter void removeItem(in DOMString key);
        void clear();
        };

* **there is a property to get the total number of values in the storage area, and to iterate through all of the keys by index (to get the name of each key).**

        interface Storage {
            readonly attribute unsigned long length;
            getter DOMString key(in unsigned long index);   
        };

----

#### TRACKING CHANGES TO THE HTML5 STORAGE AREA:

* **If you want to keep track programmatically of when the storage area changes, you can trap the storage event. The storage event is fired on the window object whenever is triggered:**
 
 1. setItem()

 2. removeItem()
 
 3. clear() 


**Example:**

    if (window.addEventListener) {
    window.addEventListener("storage", handle_storage, false);
    } else {
         window.attachEvent("onstorage", handle_storage);
    };
    

    function handle_storage(e) {
         if (!e) { e = window.event; }
    }

----

#### StorageEvent Object

| Property | Type   | Description                                                           |
|----------|--------|-----------------------------------------------------------------------|
|    key   | string | the named key that was added, removed, or modified                    |
| oldValue |   any  | the previous value (now overwritten), or null if a new item was added |
| newValue |   any  | the new value, or null if an item was removed                         |
|   url*   | string | the page which called a method that triggered this change             |

* Note: the url property was originally called uri. Some browsers shipped with that property before the specification changed. For maximum compatibility, you should check whether the url property exists, and if not, check for the uri property instead.


----

#### HTML5 Storage in Action:

**EXample**

        function saveGameState() {
            if (!supportsLocalStorage()) { return false; }
            localStorage["halma.game.in.progress"] = gGameInProgress;
            for (var i = 0; i < kNumPieces; i++) {
            localStorage["halma.piece." + i + ".row"] = gPieces[i].row;
            localStorage["halma.piece." + i + ".column"] = gPieces[i].column;
            }
            localStorage["halma.selectedpiece"] = gSelectedPieceIndex;
            localStorage["halma.selectedpiecehasmoved"] = gSelectedPieceHasMoved;
            localStorage["halma.movecount"] = gMoveCount;
            return true;
        }

        function resumeGame() {
            if (!supportsLocalStorage()) { return false; }
            gGameInProgress = (localStorage["halma.game.in.progress"] == "true");
            if (!gGameInProgress) { return false; }
            gPieces = new Array(kNumPieces);
            for (var i = 0; i < kNumPieces; i++) {
            var row = parseInt(localStorage["halma.piece." + i + ".row"]);
            var column = parseInt(localStorage["halma.piece." + i + ".column"]);
            gPieces[i] = new Cell(row, column);
            }
            gNumPieces = kNumPieces;
            gSelectedPieceIndex = parseInt(localStorage["halma.selectedpiece"]);
            gSelectedPieceHasMoved = localStorage["halma.selectedpiecehasmoved"] == "true";
            gMoveCount = parseInt(localStorage["halma.movecount"]);
            drawBoard();
            return true;
        }

----


Github Live: [view](https://anassawalha95.github.io/reading-notes-2/Class%2013)

Github Repo: [view](https://github.com/anassawalha95/reading-notes-2/blob/main/Class%2013.md)
