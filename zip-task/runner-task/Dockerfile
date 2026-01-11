FROM python:3.11

RUN useradd -m runner
RUN mkdir -p /home/runner/app
COPY app.py /home/runner/app/
RUN chown -R runner:runner /home/runner/app

USER runner
WORKDIR /home/runner/app

CMD ["python", "app.py"]
