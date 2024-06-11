# Landing page

Учебное одностраничное приложение с использованием api телеграмм-бота https://core.telegram.org/api для отправки с сайта заявок в бот, заявки остаются как в боте так и в базе данных.

## Quickstart

Run the following commands to bootstrap your environment:

    sudo apt-get install -y git python-venv python-pip
    git clone https://github.com/OlgaPertsova/Landing-page.git
    cd landing-page

    python -m venv venv
    source venv/bin/activate
    pip install -r requirements.txt

    cp .env

Run the app locally:
    
    python manage.py runserver

Run the app docker:

    git clone https://github.com/OlgaPertsova/Landing-page.git
    cd landing-page
    docker build . --tag docker-landing-page
    docker images
    docker run -p 8004:8001 image_id/image_tag
