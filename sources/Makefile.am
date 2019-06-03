MEKKI_SOURCE= \
  index.mekki \
  installing-android-sdk-cmd-line-tools.mekki

SOURCE= \
  mekki.css \
  $(MEKKI_SOURCE)

noinst_DATA = \
  $(subst .mekki,.html,$(MEKKI_SOURCE))

# flags
MEKKI_FLAGS = -t html -c mekki.css -s 1

# mekki to html
.mekki.html:
	mekki $(MEKKI_FLAGS) $< > ../docs/$*.html

# clearfiles
clean-local:
	-rm -rf ../docs/*.html
