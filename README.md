# Frith Print Queue (and other stuff) Front End

## Linux Package Requirements
npm: 9.2.0
unclutter: any version

## How-To (Run in Chrome and configure pi settings)
Setup Files
```
git clone https://github.com/ColtonTshudy/frith-printqueue-frontend/
cd frith-queue-frontend
git pull
npm i
npm run build

```

Start middleware (reverse proxy program)
```
cd src
node middleware.js

```

Start frontend
```
cd frith-printqueue-frontend/dist
python3 -m http.server 8000

```

Boot chrome
```
chromium-browser --kiosk http://localhost:8000

```

## How-To (Bare minimum or debugging)
```
cd frith-queue-frontend
sudo apt-get install npm
npm i
npm run dev

```

## Other stuff
Schedule a restart and remove mouse cursor after 10 seconds
```
sudo shutdown -r 8:00
unclutter -idle 10
```

Disable screen sleeping
```
xset s off
xset -dpms s off
set dpms 0 0 0

```
