# pc aplication version of YoyloNerd budgeting app as
## run 
~~~
cd ./server && npm install 
cd ../frontend && npm install
and run npm start in the main directory and the server directory
~~~

## frontend folder needs a .env file containing:
REACT_APP_BASE_URL=true
## server folder needs a .env file containing:
DATABASE_URL= mongo url\
OAUTH_GOOGLE_ID= google oauth id\
OAUTH_GOOGLE_SECRET= google oauth secret\
GOOGLE_REDIRECT_URL=http://localhost:5000/api/auth/google \
SESSION_SECRET= custom session secret\
DEV=true

## to run the desktop app:
install rust at: https://www.rust-lang.org/tools/install
run 
~~~
cd /frontend/src-tauri 
cargo tauri dev
~~~
NOTE: Currently all servers need ot be on for the rust app to work.
      For now it will also start up in the browser, this will be changed up on the next update.