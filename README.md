python project

backend:-

1.  Install python and pip

sudo apt update
sudo apt install -y python3 python3-pip python3-venv


2. Create a virtual environment 

cd ~/python-demoapp/src

python3 -m venv venv
source venv/bin/activate

so (venv) will create inside the server only -- for testing

pip install -r requirements.txt

uvicorn main:app --reload --host 0.0.0.0 --port 8000


after done testing in local 

deactivate




frontend:-

node.js

https://nodejs.org/en/download

# Download and install nvm:
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.2/install.sh | bash

after curl  add 3 commands which given in command promt after curl command




# in lieu of restarting the shell
\. "$HOME/.nvm/nvm.sh"
# Download and install Node.js:
nvm install 22
# Verify the Node.js version:
node -v # Should print "v22.14.0".
nvm current # Should print "v22.14.0".
# Verify npm version:
npm -v # Should print "10.9.2".


to start application:-
in frontend
npm run dev



Additonal to connect frontend and backend:-

backend:
vi .env

OPEN_API_KEY: sk-svcacct-dh4ECyHYy0oZRiFc2vmBn0s2xHvwSJNXQly2M1L0fTwFD90lD1UgKHeSSBxo-2GPSc50CX2yTLT3BlbkFJopihJ5WwNWSY-wyLMZhquZ_I1rvSM7Q3tRLetXuZCfVMh7uBVPk2ns9FEVlcQAwB4OxHtrLkw

note:
.env -- openapikey    ( create openAI key from openAI platform   - A record )


frontend:
vi .env

NEXT_PUBLIC_API_BASE_URL=http://3.83.116.79:8000

note:
.env-- url of backend for frontend





to start genAI project

in project repo:

docker-compose up


frontend:

npm run build
