FROM python:3.11

WORKDIR cralwer

ENV PYTHONUNBUFFERED=1

COPY requirements-crawler.txt .

RUN pip install --upgrade pip && pip install --no-cache-dir -r requirements-crawler.txt

COPY . .

ENTRYPOINT [ "scrapy", "crawl"]
CMD [ "104spider" ]