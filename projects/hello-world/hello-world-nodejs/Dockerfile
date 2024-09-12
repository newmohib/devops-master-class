FROM node:8.16.1-alpine
WORKDIR /app
# RUN pip install --upgrade npm for this copy and isntall form cached

COPY package.json /app
RUN npm install

# if we will update the application only we will get only update the code 
COPY . /app
EXPOSE 5000
CMD node index.js

#ENTRYPOINT ["node", "index.js"]
#COPY package.json /app
