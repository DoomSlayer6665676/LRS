┌──(doom㉿kali)-[~]
└─$ export GITHUB_USERNAME=DoomSlayer6665676                            
export GIST_TOKEN=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  
alias edit=nano  
                                                                                                                                            
┌──(doom㉿kali)-[~]
└─$ mkdir -p ${GITHUB_USERNAME}/workspace                             
                                                                                                                                            
┌──(doom㉿kali)-[~]
└─$ cd ${GITHUB_USERNAME}/workspace
                                                                                                                                            
┌──(doom㉿kali)-[~/DoomSlayer6665676/workspace]
└─$ pwd
/home/doom/DoomSlayer6665676/workspace
                                                                                                                                            
┌──(doom㉿kali)-[~/DoomSlayer6665676/workspace]
└─$ cd ..
                                                                                                                                            
┌──(doom㉿kali)-[~/DoomSlayer6665676]
└─$ pwd
/home/doom/DoomSlayer6665676
                                                                                                                                            
┌──(doom㉿kali)-[~/DoomSlayer6665676]
└─$ mkdir -p workspace/tasks/            
mkdir -p workspace/projects/
mkdir -p workspace/reports/
cd workspace
                                                                                                                                            
┌──(doom㉿kali)-[~/DoomSlayer6665676/workspace]
└─$ wget https://nodejs.org/dist/v6.11.5/node-v6.11.5-linux-x64.tar.xz
--2025-02-27 00:25:04--  https://nodejs.org/dist/v6.11.5/node-v6.11.5-linux-x64.tar.xz
Распознаётся nodejs.org (nodejs.org)… 104.20.22.46, 104.20.23.46, 2606:4700:10::6814:162e, ...
Подключение к nodejs.org (nodejs.org)|104.20.22.46|:443... соединение установлено.
HTTP-запрос отправлен. Ожидание ответа… 200 OK
Длина: 9356460 (8,9M) [application/x-xz]
Сохранение в: «node-v6.11.5-linux-x64.tar.xz»

node-v6.11.5-linux-x64.tar.xz      100%[================================================================>]   8,92M  2,47MB/s    за 3,6s    

2025-02-27 00:25:08 (2,47 MB/s) - «node-v6.11.5-linux-x64.tar.xz» сохранён [9356460/9356460]

                                                                                                                                            
┌──(doom㉿kali)-[~/DoomSlayer6665676/workspace]
└─$ tar -xf node-v6.11.5-linux-x64.tar.xz
                                                                                                                                            
┌──(doom㉿kali)-[~/DoomSlayer6665676/workspace]
└─$ rm -rf node-v6.11.5-linux-x64.tar.xz
                                                                                                                                            
┌──(doom㉿kali)-[~/DoomSlayer6665676/workspace]
└─$ mv node-v6.11.5-linux-x64 node
mv: cannot overwrite 'node/node-v6.11.5-linux-x64': Каталог не пуст
                                                                                                                                            
┌──(doom㉿kali)-[~/DoomSlayer6665676/workspace]
└─$ rm node                             
rm: невозможно удалить 'node': Это каталог
                                                                                                                                            
┌──(doom㉿kali)-[~/DoomSlayer6665676/workspace]
└─$ rm -r node   
                                                                                                                                            
┌──(doom㉿kali)-[~/DoomSlayer6665676/workspace]
└─$ mv node-v6.11.5-linux-x64 node
                                                                                                                                            
┌──(doom㉿kali)-[~/DoomSlayer6665676/workspace]
└─$ ls node/bin
node  npm
                                                                                                                                            
┌──(doom㉿kali)-[~/DoomSlayer6665676/workspace]
└─$  echo ${PATH}
/home/doom/.local/bin:/usr/local/sbin:/usr/sbin:/sbin:/usr/local/bin:/usr/bin:/bin:/usr/local/games:/usr/games:/home/doom/.dotnet/tools
                                                                                                                                            
┌──(doom㉿kali)-[~/DoomSlayer6665676/workspace]
└─$ export PATH=${PATH}:`pwd`/node/bin
                                                                                                                                            
┌──(doom㉿kali)-[~/DoomSlayer6665676/workspace]
└─$ echo ${PATH}
/home/doom/.local/bin:/usr/local/sbin:/usr/sbin:/sbin:/usr/local/bin:/usr/bin:/bin:/usr/local/games:/usr/games:/home/doom/.dotnet/tools:/home/doom/DoomSlayer6665676/workspace/node/bin
                                                                                                                                            
┌──(doom㉿kali)-[~/DoomSlayer6665676/workspace]
└─$ mkdir scripts
mkdir: невозможно создать каталог «scripts»: Файл существует
                                                                                                                                            
┌──(doom㉿kali)-[~/DoomSlayer6665676/workspace]
└─$ rm -r scripts
                                                                                                                                            
┌──(doom㉿kali)-[~/DoomSlayer6665676/workspace]
└─$ mkdir scripts
                                                                                                                                            
┌──(doom㉿kali)-[~/DoomSlayer6665676/workspace]
└─$ cat > scripts/activate<<EOF
export PATH=\${PATH}:`pwd`/node/bin
EOF
                                                                                                                                            
┌──(doom㉿kali)-[~/DoomSlayer6665676/workspace]
└─$ source scripts/activate
                                                                                                                                            
┌──(doom㉿kali)-[~/DoomSlayer6665676/workspace]
└─$ gem install gist
ERROR:  While executing gem ... (Gem::FilePermissionError)
    You don't have write permissions for the /var/lib/gems/3.1.0 directory.
        /usr/lib/ruby/vendor_ruby/rubygems/installer.rb:713:in `verify_gem_home'
        /usr/lib/ruby/vendor_ruby/rubygems/installer.rb:903:in `pre_install_checks'
        /usr/lib/ruby/vendor_ruby/rubygems/installer.rb:303:in `install'
        /usr/lib/ruby/vendor_ruby/rubygems/resolver/specification.rb:105:in `install'
        /usr/lib/ruby/vendor_ruby/rubygems/request_set.rb:195:in `block in install'
        /usr/lib/ruby/vendor_ruby/rubygems/request_set.rb:183:in `each'
        /usr/lib/ruby/vendor_ruby/rubygems/request_set.rb:183:in `install'
        /usr/lib/ruby/vendor_ruby/rubygems/commands/install_command.rb:215:in `install_gem'
        /usr/lib/ruby/vendor_ruby/rubygems/commands/install_command.rb:231:in `block in install_gems'
        /usr/lib/ruby/vendor_ruby/rubygems/commands/install_command.rb:224:in `each'
        /usr/lib/ruby/vendor_ruby/rubygems/commands/install_command.rb:224:in `install_gems'
        /usr/lib/ruby/vendor_ruby/rubygems/commands/install_command.rb:170:in `execute'
        /usr/lib/ruby/vendor_ruby/rubygems/command.rb:328:in `invoke_with_build_args'
        /usr/lib/ruby/vendor_ruby/rubygems/command_manager.rb:253:in `invoke_command'
        /usr/lib/ruby/vendor_ruby/rubygems/command_manager.rb:193:in `process_args'
        /usr/lib/ruby/vendor_ruby/rubygems/command_manager.rb:151:in `run'
        /usr/lib/ruby/vendor_ruby/rubygems/gem_runner.rb:52:in `run'
        /usr/bin/gem:12:in `<main>'
                                                                                                                                            
┌──(doom㉿kali)-[~/DoomSlayer6665676/workspace]
└─$ sudo gem install gist
[sudo] пароль для doom: 
Fetching gist-6.0.0.gem
Successfully installed gist-6.0.0
Parsing documentation for gist-6.0.0
Installing ri documentation for gist-6.0.0
Done installing documentation for gist after 0 seconds
1 gem installed
                                                                                                                                            
┌──(doom㉿kali)-[~/DoomSlayer6665676/workspace]
└─$ (umask 0077 && echo ${GIST_TOKEN} > ~/.gist)
