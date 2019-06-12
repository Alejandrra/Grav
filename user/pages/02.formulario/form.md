---
title: 'Formulario Contacto'
cache_enable: false
form:
    name: contact
    action: /formulario
    fields:
        -
            name: name
            label: Nombre
            classes: form-control
            autofocus: 'off'
            autocomplete: 'on'
            type: text
            position: left
            validate:
                required: true
        -
            name: email
            label: Email
            classes: form-control
            placeholder: 'Ingrese su email'
            type: email
            position: left
            validate:
                required: true
        -
            name: tel
            label: Teléfono
            classes: form-control
            placeholder: 'Ingrese su número celular'
            autofocus: 'off'
            autocomplete: 'on'
            type: text
            position: left
            validate:
                required: true
        -
            name: dateb
            label: 'Fecha Nacimiento'
            classes: form-control
            autofocus: 'off'
            autocomplete: 'on'
            type: date
            position: left
            validate:
                required: true
        -
            name: message
            label: Mensaje
            placeholder: 'Ingrese su mensaje'
            type: textarea
            classes: form-control
            position: right
        -
            name: genero
            label: Género
            classes: form-control
            autofocus: 'off'
            autocomplete: 'on'
            type: select
            position: right
            options:
                Masculino: Masculino
                Femenino: Femenino
                Otro: Otro
            validate:
                required: true
        -
            name: ecivil
            label: 'Estado Civíl'
            classes: form-control
            autofocus: 'off'
            autocomplete: 'on'
            type: select
            position: right
            options:
                Soltero: Soltero
                Casado: Casado
                Unión_Libre: 'Unión libre'
            validate:
                required: true
    buttons:
        -
            type: submit
            classes: 'btn btn-primary btn-lg'
            value: Enviar
    process:
        -
            email:
                subject: Mensaje
                body: '{% include ''forms/data.txt.twig'' %}'
                from: '{{ config.plugins.email.from }}'
                from_name: 'Su nombre'
                to: '{{ form.value.email|e }}'
                to_name: '{{ form.value.name|e }}'
                process_markdown: true
        -
            reset: false
---

