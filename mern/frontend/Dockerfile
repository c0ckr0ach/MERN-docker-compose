# start client:
    # cd mern/client
    # npm install
    # npm run dev
# never fetch the latest image. stick to a particular version to avoid unexpected breaking changes in the future.
FROM node:18.9.1
# make sure use a work directiory inside the container to avoid permission issues
WORKDIR /app
# copy package.json to the work directory
COPY package.json .

RUN npm install
# copy the rest of the files to the work directory
COPY . .
# expose the port that the app runs on
EXPOSE 5173

CMD ["npm", "run", "dev"]

