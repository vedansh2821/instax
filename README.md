# InstaX — InstaHak

A Dear PyGui desktop app that tries passwords from a wordlist against an
Instagram username through Instagram's web login endpoint — i.e. a
credential brute-force / password-spraying tool.

## ⚠️ Use only within the rules

- Trying passwords against an account you do not own, or without explicit
  permission, violates Instagram's Terms of Use and can be illegal. It can
  also get the account locked and the IP address rate-limited or banned.
- Only use this for authorised testing of your own account, in line with
  Instagram's terms and local law.

## Run it

```bash
git clone https://github.com/vedansh2821/instax.git
cd instax
python3 -m pip install -r requirements.txt
python3 app.py
```

Enter a username and the path to a password list (default `core/pl.txt`),
then press **start**. The app reports each tried password and stops when
one works.

## Layout

- `app.py` — Dear PyGui interface
- `core/instahak.py` — login attempts via `requests`
- `core/pl.txt` — password wordlist used by default
- `requirements.txt` — `dearpygui`, `requests`

## Requirements

- Python 3
- `dearpygui==1.6.2`, `requests`
