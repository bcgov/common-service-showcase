---
name: CDOGS
title: Common Document Generation Service
type: service
order: 10
permalink: /cdogs.html
img:
  path: /assets/images/cdogs.svg
  alt: CDOGS 
urls:
  github: https://github.com/bcgov/common-document-generation-service
  docs: https://cdogs-master-idcqvl-prod.pathfinder.gov.bc.ca/api/v2/docs  
---
<div class="row">
  <div class="col-lg-12 text-center">
          {% if page.img %}
            <img class="img-fluid" src="{{ site.baseurl }}{{page.img.path }}" alt="{{ page.img.alt }}">
          {% endif %}   
  </div>
  <div class="col-md-12">
    <div><p>Leverage your structured datasets and your business templates to automatically populate printable documents, spreadsheets, presentations, or PDFs using the Common Document Generation Service.  
    </p></div>
    <div class="h5">Capabilities</div>
    <div><p>
The API can generate any PDF or XML-based documents such as docx, xlsx, pptx, odt, ods, odp, and html. Examples of XML-based editors include Microsoft Office&#x2122;, LibreOffice&#x2122; or OpenOffice&#x2122;.
      </p>
      <p>The CDOGS API is capable of doing the following:<ol>
        <li>Merge complex datasets into document templates</li>
        <li>Supports any XML-based document templates including but not limited to Microsoft Office&#x2122;, LibreOffice&#x2122; or OpenOffice&#x2122;</li>
        <li>Rich templating library support leveraging the <a href="https://carbone.io" target="_blank">Carbone JS library</a></li>
        </ol>
      </p>
    </div>
  </div>

</div>
