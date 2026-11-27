OSAMA app - project files
=========================
index.html     the whole app (UI + logic), works alone in any browser
manifest.json  phone install info (name, icons, colors)
sw.js          offline support (service worker)
icon-*.png     phone icons (192 and 512)
icon.png/.ico  Windows icons
main.js        Electron launcher (Windows program)
package.json   Electron project settings and build command

Phone (PWA): upload index.html, manifest.json, sw.js, icon-192.png, icon-512.png
to any https host (GitHub Pages / Netlify), open the link on the phone, Add to Home Screen.

Windows program: install Node.js, put all files in one folder, then run:
  npm install
  npm start          (test)
  npm run build      (creates Setup.exe and portable .exe in the dist folder)
