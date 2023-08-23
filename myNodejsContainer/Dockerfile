# initializing a new build stage and setting node as a baseline 714
FROM node:12
# copy the package.json file from the source directory to the root of the container
COPY package*.json ./
# execute the npm install instruction to install a package its dependencies
RUN npm install
# copy all the files in the container’s filesystem 
COPY . .
# expose the port 3000
EXPOSE 3000
#provide a default argument for the entry point instruction
CMD [ “node”, “server.js” ]
LABEL org.opencontainers.image.source="https://msazure.visualstudio.com/DefaultCollection/SecurityHealthandAnalysis/_git/AymillerTest"
