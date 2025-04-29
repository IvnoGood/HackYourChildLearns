# HackYourChildLearns
I made a little hack to cheat the simple puzzle game where you have to guess countries


## How to use
Install the extension [Page Manipulator](https://github.com/Ruud14/Page-Manipulator)  from Github or from the [Chrome Web store](https://chromewebstore.google.com/detail/page-manipulator/mdhellggnoabbnnchkeniomkpghbekko) (other browsers disponible on the Github Profile).
Click on the extension logo near the address bar and open the popup. Then create a new file in js (any name) then paste the code:

    function sleep(ms) {
        return new Promise(resolve => setTimeout(resolve, ms));
    }
    
    async function demo() {
        document.getElementById("mpCountriesEasy").click();
        await sleep(1500);
        for (let i = 0; i < 52; i++) {
            console.log(`Placing piece #${i + 1}`);
            PuzzleGame.pieceSnapped();
            await sleep(1250); // Wait 1 second
        }
    }
    
    demo();
Then click on the manipulate button for the hack to start

## Features

 1. You can adjust the time between each country placement
 `await sleep(1250); <---- HERE time in ms`
 
 2. It starts the game even in the mode selection (to not loose time at lunch)

 
