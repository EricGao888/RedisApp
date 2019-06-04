# RedisApp

## Project Description
- A task manager web application based on Redis and Node.js.
- Adding and deleting tasks are supported.

## Configuration
- Download Redis from its official website.
- Use `make install` to install Redis directly into your system.
- Run `redis-server` to start Redis.
- Run `redis-cli` in another terminal to use redis client.
- Run `npm install` to install dependencies included in the `package.json` file.

## Development Diary
- Dependencies are provided in file `package.json`.
- Callback function: `Function` is `Object`, every function is actually an instance of `Function` class. A function can be used as an argument or return value of another function. Function name is acutally a `pointer` pointing to the function.

## Trouble Shooting

### nodemon Intallation Trouble
- To avoid restarting the sever every time we modify the app.js(backend) file, I executed `sudo npm install nodemon -g` to install `nodemon` globally but got `EACCES` error. I solved the problem as follows(still got error but nodemon could be used after those changes):
- `npm config set prefix /usr/local`
- `sudo npm install nodemon -g --registry=https://registry.npm.taobao.org`

### Can not Shutdown Redis
- Execute `shutdown nosave` in `redis-cli`.
