# TP1-watermark-project-


•	Étape 1 : importer le watermark sur l’image 
Via la librairie  PIL  et la fonction watermark.picture (on peut dès lors importer le watermark sur l’image . cette fonction permet de construire via 2 image une image de sortie.

def :watermark_picture(input_image_path,output_image_path,watermark_image_path,position)

•	Étape 2 : positionner le watermark sur l’image ou on le désire 

Pour la position du watermark sur l image la même fonction « watermark_picture » permet aussi par , position (x,y) afin de  déterminer l’emplacement décisé du watermark.
 
def watermark_picture(input_image_path,output_image_path,watermark_image_path,position)

•	Étape 3 : pixels blanc uniquement pour le watermark 

Via la librairie PIL l’image ne montre pas directement les pixels on doit dès lors convertir 
l’image en mode RGBA et ainsi extraire les pixels via la liste newData[]. 
On a donc accès aux pixels de l’image, celle-ci étant en noir et blanc donc binaire on donne 
comme  condition  R<150 ( valeur des blanc)

•	Étape 4-> transparence du watermark . 
pour cela même structure que pour les pixels blanc  c’est-à-dire RGBA avec le rajout de la fonction im.putalpha  qui nous permet de choisir la texture im.putalpha (128)




Sources utilisées :

https://note.nkmk.me/en/python-pillow-putalpha/
https://www.blog.pythonlibrary.org/2017/10/17/how-to-watermark-your-photos-with-python/
https://f-legrand.fr/scidoc/srcdoc/image/extraction/regions/regions-pdf.pdf
