apt-get update

echo "deb http://http.kali.org/kali kali-rolling main non-free contrib" | sudo tee /etc/apt/sources.list

echo "deb-src http://http.kali.org/kali kali-rolling main non-free contrib" | sudo tee /etc/apt/sources.list

gpg --keyserver hkp://keys.gnupg.net --recv-key ED444FF07D8D0BF6

gpg -a --export ED444FF07D8D0BF6 | apt-key add -




wget -q -O - https://archive.kali.org/archive-key.asc  | apt-key add
