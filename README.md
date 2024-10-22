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
<br><br>

## <div align="center">⚙️ Configuration</div>

The configuration file allows you to customize the server settings, such as:

- Listening ports
- Root directory for serving files
- Error pages
- Request limits

<br>See the config.conf file to see what you can change.
<br>More information is available in the subject.