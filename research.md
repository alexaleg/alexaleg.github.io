---
layout: page
permalink: /research/
title: Research
books:
    - title:   "Process Analysis and Simulation in Chemical Engineering"
      author:  "Gil Chaves, I.D., López, J.R.G., García Zapata, J.L., Leguizamón Robayo, A., Rodríguez Niño, G."
      journal: "Springer International Publishing"
      <>note:  "(presented at Oz)"
      year:    "2016"
      image:   "/images/books/PAiChE.webp"
      url:     "https://www.springer.com/gp/book/9783319148113"
      doi:     "http://dx.doi.org/10.1007/978-3-319-14812-0"
    - title:   "Análisis y Simulación de Procesos en Ingeniería Química"
      author:  "Gil Chaves, I.D., López, J.R.G., García Zapata, J.L., Leguizamón Robayo, A."
      journal: "Editorial UN"
      <>note:  "Coleción 150 años Facultad de Ingeniería"
      year:    "2011"
      image:   "/images/books/ASPIngQ.webp"
      url:     "https://www.libreriadelau.com/analisis-y-simulacion-de-procesos-en-ingenieria-quimica/p"
      <>doi:     "http://dx.doi.org/10.1007/978-3-319-14812-0"
pubs:
    - title:   "Approximate Constrained Lumping of Polynomial Differential Equations"
      author:  "Leguizamon-Robayo, A., Jiménez-Pastor, A., Tribastone, M., Tschaikowski, M., Vandin, A."
      journal: "Lecture Notes in Computer Science"
      note:    "Conference Computational Methods in Systems Biology"
      year:    "2023"
      url:     "https://link.springer.com/chapter/10.1007/978-3-031-42697-1_8"
      doi:     "https://doi.org/10.1007/978-3-031-42697-1_8"
    - title:   "Minimization of Dynamical Systems over Monoids"
      author:  "G. Argyris, A. L. Lafuente, A. L. Robayo, M. Tribastone, M. Tschaikowski and A. Vandin"
      journal: "Lecture Notes in Computer Science"
      note:    "38th Annual ACM/IEEE Symposium on Logic in Computer Science (LICS), pp. 1-14"
      year:    "2023"
      url:     "https://ieeexplore.ieee.org/abstract/document/10175697"
      doi:     "https://doi.org/10.1109/LICS56636.2023.10175697"
    - title:   "Efficient Estimation of Agent Networks"
      author:  "Leguizamon-Robayo, A., Tschaikowski, M."
      journal: "Lecture Notes in Computer Science"
      note:    "Conference ISoLA."
      year:    "2022"
      url:     "https://link.springer.com/chapter/10.1007/978-3-031-19759-8_13"
      doi:     "https://doi.org/10.1007/978-3-031-19759-8_13"
    - title:   "Control of an azeotropic distillation process to acetonitrile production"
      author:  "Ruiz, A., Borda, N., Leguizamón, A., Guevara, J. R., Gil C., I.D."
      journal: "Computer Aided Chemical Engineering"
      note:    "Volume 29, Pages 833-838"
      year:    "2011"
      url:     "https://www.sciencedirect.com/science/article/pii/B978044453711950167X?via%3Dihub"
      doi:     "https://doi.org/10.1016/B978-0-444-53711-9.50167-X"
      <>media:
      <> - name: "IMDB"
      <>    url:  "http://www.imdb.com/title/tt0133093/"

---

# Publications
{% assign thumbnail="left" %}

{% for pub in page.pubs %}

{% if pub.image %}
{% include image.html url=pub.image caption="" height="100px" align=thumbnail %}
{% endif %}
[**{{pub.title}}**]({% if pub.internal %}{{pub.url | prepend: site.baseurl}}{% else %}{{pub.url}}{% endif %}){:target="_blank"}<br />
{{pub.author}}<br />
*{{pub.journal}}*
{% if pub.note %} *({{pub.note}})*
{% endif %} *{{pub.year}}* {% if pub.doi %}[[doi]({{pub.doi}})]{% endif %}
{% if pub.media %}<br />URL: {% for article in pub.media %}[[{{article.name}}]({{article.url}})]{% endfor %}{% endif %}

{% endfor %}

# Books 
{% assign thumbnail="left" %}

{% for book in page.books %}
{% if book.image %}
{% include image.html url=book.image caption="" height="100px" align=thumbnail %}
{% endif %}
[**{{book.title}}**]({% if book.internal %}{{book.url | prepend: site.baseurl}}{% else %}{{book.url}}{% endif %}){:target="_blank"}<br />
{{book.author}}<br />
*{{book.journal}}*
{% if book.note %} *({{book.note}})*
{% endif %} *{{book.year}}* {% if book.doi %}[[doi]({{book.doi}})]{% endif %}
{% if book.media %}<br />URL: {% for article in book.media %}[[{{article.name}}]({{article.url}})]{:target="_blank"}{% endfor %}{% endif %}
{% endfor %}
<br/>

# Theses 
* MSc Pure Mathematics - [On Moment Maps and Jacobi Manifolds](https://repositorio.unal.edu.co/bitstream/handle/unal/79669/EncabezadoTesisMSc.pdf?sequence=2&isAllowed=y){:target="_blank"}. 
* MSc Chemical Engineering - [Optimal Operation of Small LNG Refrigeration Cycles](https://ntnuopen.ntnu.no/ntnu-xmlui/handle/11250/2413532){:target="_blank"}.
