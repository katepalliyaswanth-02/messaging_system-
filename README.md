# messaging_system-

1.Clone the Repository

git clone https://github.com/katepalliyaswanth-02/messaging_system-.git
cd messaging_system

2.Create a Virtual Environment

python3 -m venv yash
source yash/bin/activate

3.Install dependencies

pip install -r requirements.txt

4.install RabbitMQ

sudo apt update
sudo apt install rabbitmq-server -y
sudo systemctl enable rabbitmq-server
sudo systemctl start rabbitmq-server
sudo systemctl status rabbitmq-server
sudo rabbitmqctl status
sudo rabbitmq-plugins enable rabbitmq_management
sudo systemctl restart rabbitmq-server

Then open in you browser
http://localhost:15672/
Default-username,password=guest

5.Runs on flask app
python3 app.py

6.Install celery

pip install celery

7.Run on celery worker

In another terminal activate venv again
source yash/bin/activate

Then start the celery worker

celery -A app.celery worker --loglevel=info


8.pip install grok

add ngrok authtoken  token_here

9.Expose server using ngrok

ngrok http 5000

Ngrok will provide a public URL like:

https://example-tunnel.ngrok-free.app

10.Get messages
curl http://127.0.0.1:5000/messages

<img width="1848" height="945" alt="Screenshot 2025-10-05 194223" src="https://github.com/user-attachments/assets/5a225e46-d7ac-4122-9c13-af3e389cc2f8" />

<img width="1916" height="874" alt="image" src="https://github.com/user-attachments/assets/066e7fd2-4afe-4580-aa50-6e5830016ee7" />

<img width="1919" height="960" alt="image" src="https://github.com/user-attachments/assets/cb855393-a439-4224-8dd2-322ba0fd2308" />



