# A Flask Web App for Generating Text with [GPT-2](https://github.com/openai/gpt-2)

GPT-2, a very large language model hyped as too dangerous to release its full version, can generate realistic text close to human level based on its input. I have tweaked this version to run off the full 1558M parameter version. But you will need a big instance to run this on. I have only tested it on [DigitalOcean](https://m.do.co/t/b298d6966c0c) (signup with my referral link, I get some free credits) 16GB Ubuntu 18.04 which cost $80 a month. And it is not fast. 


## Demo
![Demo](demo.png)



## Usage
1. Clone the repository.
    ```
    $ git clone https://github.com/eplt/gpt2-app.git
    ```

2. Build a new Docker image from [`Dockerfile`](https://github.com/eplt/gpt2-app/blob/master/Dockerfile).
    ```
    $ cd gpt2-app
    $ docker build -t gpt2-app:0.1-py3 --rm .
    ```

3. Run the app in a container.
    ```
    $ docker run -p 5000:5000 --name gpt2-app gpt2-app:0.1-py3
    ```

4. Navigate to the page where the app is hosted. (e.g. `127.0.0.1:5000` for local deployment, or `ip:5000` for remote servers)



## License

[MIT](https://github.com/jingw222/gpt2-app/blob/master/LICENSE)







