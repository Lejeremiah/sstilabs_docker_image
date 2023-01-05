FROM python:3.7-alpine
COPY ./app /app
WORKDIR /app
RUN pip install -r requirements.txt
CMD sh -c "echo $FLAG > /flag && export FLAG=not_flag && FLAG=not_flag" \
    && python app.py
EXPOSE 5000