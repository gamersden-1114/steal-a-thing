# Steal a Thing

A chaotic browser game about collecting oddball characters, building a base, and raiding NPC bases.

## Play

Open the [GitHub Pages site](https://gamersden-1114.github.io/steal-a-thing/). Create an account with an email, password, and unique username, or sign in. Your coin balance, collection, and discovery index save to Firebase and follow your account across devices.

To play with a friend, choose **Play with friends → Create a game** and send them the six-character code. They sign in, choose **Join**, and enter your code.

## Controls

- **Move:** WASD, arrow keys, or drag on desktop; use the on-screen joystick on touchscreens.
- **Interact:** E on desktop or tap nearby characters/items on touchscreens.
- **Lock your base:** use the lock button near the bottom left.
- **Sell a collection item:** R near one of your occupied slots, or tap it.
- **Fullscreen / collection index:** F / I on desktop; use the corner buttons on touchscreens.

## Hosting and backend

The game is a static HTML app hosted by GitHub Pages. Firebase Authentication (email/password) and Realtime Database (accounts, saves, and friend rooms) run on the Firebase Spark plan. The browser Firebase config is public by design; database rules restrict profile writes to each signed-in user and room presence writes to the member's own account.

GitHub Actions deploys the repository root to Pages when a commit reaches `main`. No build step is required.

## Limitations

This is a lightweight friends game. Room codes are invite-only, and the game currently supports up to eight player bases per room. Progress is stored under a user's account, but game actions run in the browser, so stats are not cheat-proof. Firebase's free plan has usage limits that can change.

