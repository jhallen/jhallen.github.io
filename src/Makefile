

HTDOCS = index.html verifone.html acoustic.html relay.html editorperformance.html mpl.html capsense.html

GIFS =

all : ${HTDOCS}

publish : ${HTDOCS} ${GIFS}
	cp ${HTDOCS} ${GIFS} ..

clean :
	/bin/rm -f ${HTDOCS}

index.html : header-src.html index-src.html footer-src.html
	sed "s,@title@,Joe's Projects," <header-src.html | cat - index-src.html footer-src.html > $@

verifone.html : header-src.html verifone-src.html footer-src.html
	sed "s,@title@,The Verifone ZON Jr XL," <header-src.html | cat - verifone-src.html footer-src.html > $@

relay.html : header-src.html relay-src.html footer-src.html
	sed "s,@title@,Single Board Relay Computer," <header-src.html | cat - relay-src.html footer-src.html > $@

acoustic.html : header-src.html acoustic-src.html footer-src.html
	sed "s,@title@,Acoustic delay line memory," <header-src.html | cat - acoustic-src.html footer-src.html > $@

editorperformance.html : header-src.html editorperformance-src.html footer-src.html
	sed "s,@title@,Text Editor Performance Comparison," <header-src.html | cat - editorperformance-src.html footer-src.html > $@

mpl.html : header-src.html mpl-src.html footer-src.html
	sed "s,@title@,MPL," <header-src.html | cat - mpl-src.html footer-src.html > $@

capsense.html : header-src.html capsense-src.html footer-src.html
	sed "s,@title@,MPL," <header-src.html | cat - capsense-src.html footer-src.html > $@
