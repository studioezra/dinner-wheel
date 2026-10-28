# Dinner Spin Wheel

A single-page "what's for dinner?" wheel. Tap **Spin** and it picks a meal from your list.

- Toggle categories on and off with the chips above the wheel.
- **Not this week** takes the current pick off the wheel and spins again.
- **Manage** lets you add, edit, delete and untick meals, and add, rename or remove categories.
- The list is shared: it's stored in Firebase Firestore (document `meals/main`), so changes show up for everyone with the link. A copy is also kept in the browser (localStorage) as a fallback. **Restore original list** brings back the starting 24 meals for everyone.
- Firestore rules must allow read/write on `meals/{meal}`. Anyone with the link can edit the list.

## Run it

It's one file with no build step. Open `index.html` in a browser, or turn on GitHub Pages for this repo (Settings → Pages → deploy from the `main` branch) to get a link you can open on your phone.
