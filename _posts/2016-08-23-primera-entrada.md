---
title: Primera Entrada!
layout: single
excerpt: "Este es un texto resumen."
---


Esta página fue creada con [Jekyll](https://jekyllrb.com) y GitHub utilizando el theme [Minimal Mistakes](https://mmistakes.github.io).

![image-left](/images/jekyll-logo.png)


Jekyll is a simple, blog-aware, static site generator. It takes a template directory containing raw text files in various formats, runs it through a converter (like Markdown) and our Liquid renderer, and spits out a complete, ready-to-publish static website suitable for serving with your favorite web server. Jekyll also happens to be the engine behind GitHub Pages, which means you can use Jekyll to host your project’s page, blog, or website from GitHub’s servers for free.

```javascript
$('#otorgarLicencia').on('click', function() {
    var agente = $('#apellido_nombre_modal').val();
    var licencia = $("[name='tipo_licencia_id'] :selected").text();
    var dias = $('#cant_dias').val();
    var motivo = $('#motivo_otorgamiento').val();
    if ((dias=='')||(motivo=='')){
      swal('Asegúrese de completar los campos: "Días a otorgar" y "Motivos" ');
      return false;
    }
    swal({
      title: "Otorgamiento de Licencia",
      text: "Está seguro que desea otorgar "+dias+" días de licencia  '"+licencia+"' al Agente: "+agente+"?",
      showCancelButton: true,
      cancelButtonText: "No",
      confirmButtonColor: "#456125",
      confirmButtonText: "Si",
      closeOnConfirm: true
    },
    function(isConfirm){
        if (isConfirm){
             $('#otorgarDiasLicencia').trigger('submit');
          }
      });
});
```







