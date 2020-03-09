TITLE="mnmlst.design | design systems"

SIZES= 148 256 448 768

IMAGES=\
	448/BarSeries.png \
	448/Button.png \
	768/OI-Patternbook.png \
	768/RegionSeries.png \
	768/form.png \
	448/image.png \
	448/message.png

all: dirs $(IMAGES)

dirs: $(SIZES)

clean:
	rm -rf $(SIZES)

CNV-ARGS= -caption $(TITLE)

768/% : fullsize/%
	convert -resize 1536 $(CNV-ARGS) $< $@

448/% : fullsize/%
	convert -resize 896 $(CNV-ARGS) $< $@

256/% : fullsize/%
	convert -resize 512 $(CNV-ARGS) $< $@

224/% : fullsize/%
	convert -resize 448 $(CNV-ARGS) $< $@


$(SIZES): % :
	mkdir $@
