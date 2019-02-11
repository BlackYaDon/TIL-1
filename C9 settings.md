# C9 settings

1. python 설치

   ```python
   git clone https://github.com/pyenv/pyenv.git ~/.pyenv
   echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.bashrc
   echo 'export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.bashrc
   echo -e 'if command -v pyenv 1>/dev/null 2>&1; then\n  eval "$(pyenv init -)"\nfi' >> ~/.bashrc
   
   source ~/.bashrc
   pyenv install 3.6.7
   pyenv global 3.6.7
   python -V
   pip install --upgrade pip
   ```

2. pyenv

   ```bash
   git clone https://github.com/pyenv/pyenv-virtualenv.git $(pyenv root)/plugins/pyenv-virtualenv
   echo 'eval "$(pyenv virtualenv-init -)"' >> ~/.bashrc
   exec "$SHELL"
   ```

3. git config

   ```
   git config --global user.name edutak
   git config --global user.email edutak.ssafy@gmail.com
   ```

4. 