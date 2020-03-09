TITLE="mnmlst.design | environment design"

SIZES= 192 256 448 768

IMAGES=\
  768/garage.jpg \
  256/interior2.png \
  448/iso-struct.png \
  768/metro-ed-forensics-05.jpg \
  256/metro-ed-hallway.jpg \
  448/metro-ed-shop-05.jpg \
  448/rooftop.jpg \
  768/scene3.png \
  448/sec-bed.png \
  256/small11.png \
  256/small6.png \
  192/tes001.jpg

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

192/% : fullsize/%
	convert -resize 384 $(CNV-ARGS) $< $@

$(SIZES): % :
	mkdir $@
