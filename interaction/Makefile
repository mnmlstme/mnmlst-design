TITLE="mnmlst.design | interaction design"

SIZES= 192 256 448 768

IMAGES=\
	256/AirbusPartnershipStoryboard2.png \
	768/AirbusPartnershipStoryboard.png \
	192/1-ServiceAccounts.png \
	192/10-ServiceAccounts.png \
	192/11-ServiceAccounts.png \
	192/11a-ServiceAccounts.png \
	192/12-ServiceAccounts.png \
	192/13-ServiceAccounts.png \
	192/14-ServiceAccounts.png \
	192/15-ServiceAccounts.png \
	192/16-ServiceAccounts.png \
	192/17-ServiceAccounts.png \
	192/18-ServiceAccounts.png \
	192/2-ServiceAccounts.png \
	192/3-ServiceAccounts.png \
	192/4-ServiceAccounts.png \
	192/5-ServiceAccounts.png \
	192/9-ServiceAccounts.png \
	256/AddApp-phone-hor.png \
	192/AddApp-phone.png \
	768/Admin-dashboard.png \
	256/App-details-phone-hor.png \
	192/App-details-phone.png \
	768/App-details-tablet.png \
	256/Frequencies.png \
	448/Launcher-phone-hor.png \
	192/SourceSelected,Panelclosed.png \
	192/SourceSelected,PanelopentoConnection.png \
	192/SourceSelected,PanelopentoParser,VerticalSchema,EditingFieldInline.png \
	192/SourceSelected,PanelopentoParser,VerticalSchema.png \
	448/SourceSelected,PanelopentoParser.png \
	448/ViewSelected,PanelopentoDefinition.png


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

192/%: fullsize/%
	convert -resize 296 $(CNV-ARGS) $< $@

$(SIZES): % :
	mkdir $@
