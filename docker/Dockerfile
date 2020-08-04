FROM python:3

ADD covid-qa-chatbot.py /
ADD news.csv /
ADD multilingual.csv /
ADD community.csv /

RUN pip install swifter spacy spacy_universal_sentence_encoder nltk pyfiglet termcolor colorama
RUN python -m spacy download en_core_web_lg
RUN apt-get update && apt-get install vim -y

CMD ["python", "covid-qa-chatbot.py"]