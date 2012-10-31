include depends.mk

SOURCE=../../

CONFIGURE=./configure --prefix=$(PREFIX) --build=$(BUILD) --host=$(HOST)

all: configure
	cd $(SOURCE); make -j $(JOBS)
	cd $(SOURCE); make install
	cd $(SOURCE); make zip

clean:
distclean:
	cd $(SOURCE);

configure:
	cd $(SOURCE); ./bootstrap
	cd $(SOURCE); $(CONFIGURE)
