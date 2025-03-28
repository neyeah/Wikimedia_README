# Wikimedia_README
A README file detailing my project


**PetScan Cat-a-lot Integration: Implementation Details**

I've completed the integration of PetScan with Cat-a-lot to make categorizing Wikimedia Commons images more efficient. This project involved creating a userscript that allows users to input PetScan query IDs, fetch image lists, and display them for categorization using the existing Cat-a-lot interface.

### Implementation Approaches

I used two methods to implement this solution:

1. **Tampermonkey Userscript**: Initially, I developed and tested the script using Tampermonkey, which allowed for quick iterations and debugging. This approach is ideal for personal use or for users who prefer browser extensions.
2. **MediaWiki Integration**: For broader accessibility, I've also made the script available directly on Wikimedia Commons. This allows users to add it to their common.js without requiring any browser extensions.


### How to Test the Script

**Option 1: MediaWiki Integration (Recommended)**

1. Visit: [https://commons.wikimedia.org/wiki/User:Nenyee/PetScan-Cat-a-lot-Integration.js](https://commons.wikimedia.org/wiki/User:Nenyee/PetScan-Cat-a-lot-Integration.js)
2. Add this line to your common.js page (at User:YourUsername/common.js):

```javascript
mw.loader.load('https://commons.wikimedia.org/wiki/User:Nenyee/PetScan-Cat-a-lot-Integration.js');
```


3. Visit [https://commons.wikimedia.org/wiki/Special:BlankPage/Cat-a-lot](https://commons.wikimedia.org/wiki/Special:BlankPage/Cat-a-lot) to use the tool


**Option 2: Tampermonkey Installation**

1. Install Tampermonkey browser extension if you don't have it
2. Create a new script in Tampermonkey
3. Copy the code from: [https://commons.wikimedia.org/wiki/User:Nenyee/PetScan-Cat-a-lot-Integration.js](https://commons.wikimedia.org/wiki/User:Nenyee/PetScan-Cat-a-lot-Integration.js)
4. Save the script
5. Visit [https://commons.wikimedia.org/wiki/Special:BlankPage/Cat-a-lot](https://commons.wikimedia.org/wiki/Special:BlankPage/Cat-a-lot) to use the tool


### Features

The script provides a simple interface where you can:

- Enter a PetScan query ID
- Set an image limit (default 100)
- Access advanced options for categories, negative categories, and depth
- View a link to the original PetScan query
- See images displayed in a grid layout
- Use Cat-a-lot to categorize the displayed images


If Cat-a-lot doesn't automatically recognize the images, the script provides a fallback option to create a temporary page where Cat-a-lot will work properly.

I welcome any feedback or suggestions for improvements to make this tool more useful for the Wikimedia Commons community.
