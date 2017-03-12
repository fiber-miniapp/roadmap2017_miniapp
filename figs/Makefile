PDF_XBB := $(patsubst %.pdf,%.xbb,$(wildcard *.pdf))
PNG_XBB := $(patsubst %.png,%.xbb,$(wildcard *.png))
JPG_XBB := $(patsubst %.jpg,%.xbb,$(wildcard *.jpg))
ALL = $(PDF_XBB) $(PNG_XBB) $(JPG_XBB)

.SUFFIXES: .png .pdf .xbb .jpg
.png.xbb:
	ebb -x $<

.pdf.xbb:
	extractbb $<

.jpg.xbb:
	extractbb $<

all: $(ALL)

clean:
	rm -rf *.xbb

