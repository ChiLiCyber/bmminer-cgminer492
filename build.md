
git clone https://github.com/Zwilla/bmminer-cgminer492

cd bmminer-cgminer492

chmod -R 777 *

./autogen.sh

./configure --enable-bitamin-c5

make

now copy the file to your miner

/usr/bin

do this:

mv /usr/bin/bmminer /usr/bin/bmminer-old

cp cgminer /usr/bin/bmminer

chmod 755 /usr/bin/bmminer

/etc/init.d/bmminer.sh restart

sleep 3

screen -r

If you want to use your old bmminer, just run this

mv /usr/bin/bmminer-old /usr/bin/bmminer

/etc/init.d/bmminer.sh restart