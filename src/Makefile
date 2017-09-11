

HTDOCS = index.html verifone.html acoustic.html

GIFS = 

all : ${HTDOCS}

publish : ${HTDOCS} ${GIFS}
	cp ${HTDOCS} ${GIFS} ..

clean :
	/bin/rm -f ${HTDOCS}

index.html : header-src.html index-src.html footer-src.html
	sed "s,@title@,Relay Trainer," <header-src.html | cat - index-src.html footer-src.html > $@

verifone.html : header-src.html verifone-src.html footer-src.html
	sed "s,@title@,The Verifone ZON Jr XL," <header-src.html | cat - verifone-src.html footer-src.html > $@

acoustic.html : header-src.html acoustic-src.html footer-src.html
	sed "s,@title@,Acoustic delay line memory," <header-src.html | cat - acoustic-src.html footer-src.html > $@
