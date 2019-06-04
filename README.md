# RedisApp

## Project Description
- A task manager web application based on Redis and Node.js.
- Adding and deleting tasks are supported.

## Configuration
- Download Redis from its official website.
- Use `make install` to install Redis directly into your system.
- Run `redis-server` to start Redis.
- Run `redis-cli` in another terminal to use redis client.

## Development Diary
- Dependencies are provided in file `package.json`.
- Callback function: `Function` is `Object`, every function is actually an instance of `Function` class. A function can be used as an argument or return value of another function. Function name is acutally a `pointer` pointing to the function.