TITLE="mnmlst.design | product design"

SIZES= 224 256 448 768

IMAGES=\
	256/Branching.png \
	768/CFE_Geo_1.png \
	256/CFE_Geo_2.png \
	256/CFE_Geo_3.png \
	256/Downloads.png \
	448/IDE.png \
	768/Port_Monitoring_with_Bar_chart.png \
	448/Product_Overview.png \
	224/Progress_by_Stage.png \
	448/Timeline_sketch.jpeg \
	448/Under_the_Hood@2x.png \
	448/Working_with_Notebook@2x.png \
	768/Working_with_SQL@2x.png \
	256/graph_with_gantt_chart_and_view_details.png

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
