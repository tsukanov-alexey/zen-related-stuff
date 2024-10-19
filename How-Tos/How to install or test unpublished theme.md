# How to install or test unpublished theme

1. Locate your Zen profile directory:
    1. Open Zen browser
    2. Type `about:profiles` in address bar and press <kbd>Enter</kbd>
    3. Find table where row "Default Profile" is "true"
    4. Find in this table "Root Directory" row and click "Open Folder" button
2. Copy (or create symlink) here `<theme ID>` directory (with .css and other files) in `./chrome/zen-themes`
3. Return back into your profile directory
4. Open `./zen-themes.json` with any text editor
5. Paste this piece of JSON and replace all angle brackets fields with your data (don't forget about comma before this part):

    ```json
    "<theme ID (same as your project directory)>": {
        "id": "<theme ID (same as above)>",
        "name": "<your theme name>",
        "description": "remove if not needed",
        "style": "<URI to chrome.css>",
        "readme": "<URI to readme.md, remove if not needed>",
        "image": "<URI to image.png (300x200), remove if not needed>",
        "preferences": "<URI to preferences.json, remove if not needed>",
        "author": "John Doe",
        "version": "1.0.0",
        "tags": [],
        "createdAt": "2024-10-19",
        "updatedAt": "2024-10-19",
        "enabled": true
    }
    ```

6. Open/Refresh `Settings -> Zen Mods` page in Zen browser
7. Now you can change settings & enable or disable your theme
8. ???
9. PROFIT
