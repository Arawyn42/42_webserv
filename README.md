<div align="center">
  <h1>⚙️ webserv (a <a href="https://42perpignan.fr/">42</a> project) ⚙️</h1>
  <img src="ressources/preview.gif" alt="Preview">
  <p><b>Subject (in french):</b> <a href="ressources/fr.subject.pdf">fr.subject.pdf</a></p>
</div>
<div align="center">
  <h2>✅ Grade</h2>
  <img src="ressources/grade.png" alt="Grade">
</div><br>

## <div align="center">📄 Introduction</div>
Webserv is a C++ HTTP server project aimed at understanding the fundamentals of networking and the HTTP/1.1 protocol. It handles multiple types of requests (GET, POST, DELETE) and supports concurrent connections.

The goal of this project is to deepen knowledge of how web servers operate and handle requests from multiple clients.

The bonus part consist in handling multiple CGIs and user sessions with cookies.

For this project, we were a group of 3 students. Special thanks to [Nicolas](https://github.com/Floperatok) and [Samuël](https://github.com/MaitreOg)!
<br><br>

## <div align="center">🛠️ Features</div>
- **HTTP/1.1** compliant
- Supports **GET**, **POST**, and **DELETE** methods
- Serves static files and dynamic content
- **Concurrent connection handling** (via select/poll)
- Supports **CGI Scripts** (BONUS)
- Supports **Cookies** (BONUS)
- Configurable through external configuration files (like nginx does)
<br><br>

## <div align="center">💻 Usage</div>
To run this project, follow the steps below:

## Build and run
Clone the repository:
```sh
git clone https://github.com/Arawyn42/42_webserv webserv
```
<br>Enter the directory:
```sh
cd webserv
```
<br>Build the server:
```sh
make && make clean
```
<br>Run the server with a configuration file of your choic:
```sh
./webserv Config/config.conf
```
<br>Or use the default configuration file:
```sh
./webserv
```

## Connect to the static website
A website is already given in the www folder. So you can use it or another one of your choice (it has to be html/css).
<br>If you use a custom website, don't forget to specify the root directory and the index in your config file.

To connect to the server and see the website content, open a browser (like Google Chrome or Mozilla Firefox) and use the host and the port specified in the config file.
<br>For exemple, if the host is 127.0.0.1 (localhost) and the port (listen in config file) is 8451, you can type in the address bar:
```
http://localhost:8451
```

You can now navigate on the website. You'll see the server logs in the terminal you used to run it.
<br><br>

## <div align="center">⚙️ Configuration</div>

The configuration file allows you to customize the server settings, such as:

- Listening ports
- Root directory for serving files
- Error pages
- Request limits

<br>See the config.conf file to see what you can change.
<br>More information is available in the subject.