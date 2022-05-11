# PDF 操作


## PDF to JPG

/etc/ImageMagick-7/policy.xml

<policy domain="coder" rights="read|write" pattern="PDF" />




## PDF to SVG

dvisvgm --pdf --optimize --output=Out.svg In.pdf
