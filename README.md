# streamlit_to_heroku
stramlit

```python
Porcfile
web: sh setup.sh && streamlit run app.py

setup.sh
mkdir -p ~/.streamlit/

echo "\
[general]\n\
email = \"註冊的信箱\"\n\
" > ~/.streamlit/credentials.toml

echo "\
[server]\n\
headless = true\n\
enableCORS=false\n\
port = $PORT\n\
" > ~/.streamlit/config.toml

```python
