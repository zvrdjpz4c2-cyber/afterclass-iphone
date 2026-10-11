# Afterclass for iPhone

A small SwiftUI and WebKit app for https://study-1.floot.app. Requires iOS 16 or later and an internet connection. The app keeps its own sign-in between launches. Canvas links open in your browser.

The source contains the public app URL and icon only. Grades, homework, class notes, flashcards and saved study sessions live in the private authenticated backend, not in this repository or IPA.

## Cloud build

Run the manual GitHub Actions workflow. It builds a real arm64 iPhone app on a macOS runner and creates Afterclass-unsigned.ipa. Download the artifact and sign/install using your existing installer. This workflow does not ask for Apple account details or signing secrets.

## Local build

If you have full Xcode with the iPhone SDK, run Build IPA.command. Command Line Tools alone cannot compile an iPhone app.

## First use

Use Forgot password? with the owner's account email to set an Afterclass password. Choose Today, start a focus session, then save the session. You can save notes per class and create flashcards for review. The existing daily Canvas check updates the app at 4 PM when Codex and signed-in Chrome are available. Your own Done marks do not submit Canvas assignments.
