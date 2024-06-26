# Introdução ao HTML

- **HTML**:  *HyperText Markup Language*
- **Hipertexto** é um termo da semiótica (Ciência que estuda a comunicação) que significa que, diferentemente de um texto comum, ele pode conter referências navegáveis para outros textos.
- Essas referências são o que chamamos de **links**.
- Na semiótica é comum considerar praticamente a web inteira como um único hipertexto.
- Dizemos isso para dar um pouco de contexto, mas o que nos interessa mais como programadores é o *Markup.*
- Uma linguagem de marcação é uma linguagem que possue símbolos especiais que indicam **metainformações**.
- Elas referem-se à forma, hierarquia, ordem e/ou semântica dos elementos da página.
- Atualmente está na versão 5 (2014)

## Tags

- Marcação → **tags**
- Delimitadas por `<` e `>`;
- Usadas para descrever o elemento que será adicionado;
- Exemplo de Tags HTML:
    - `<button>`
    - `<p>`
    - `<i>`

<aside>
💡 **Exemplo**: Para pedir para o navegador exibir um (elemento) botão, podemos fazer:

```html
<button> Clique Aqui </button>
```

</aside>

## Elementos

- Geralmente contém três componentes:
    
    ![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/120b5c8b-202a-47d6-b180-84487b666423/06da3eb1-89ee-4b1a-b1eb-f1ba8025d7ad/Untitled.png)
    
    - Tag de abertura;
    - Conteúdo;
    - Tag de fechamento.
- Possui um tipo (ex.: Botão, parágrafo, imagem, lista, tabela);
- A representação textual de um elemento em código HTML é chamada **tag**;
- Grande parte dos elementos HTML permite que outros elementos sejam declarados em seu interior. Outros permitem apenas elementos específicos ou texto e outras ainda não permitem que nada seja colocado entre suas tags, esses têm a tag fechada nela mesmo.
- Elemntos também podem ter informações adicionais chamadas de atributos.
    - **Atributos** são pares chave-valor, separados por `=` e os valores devem estar envoltos em aspas;
    - Alguns atributos podem ser usados em qualquer alemento como, por exemplo, `style` que nos permite usar **CSS** para estilizar, ou `id` que provê uma identificação única para o elemento;
    - Outros são específicos de determinados elementos, por exemplo, uma imagem pode ter uma altura (`height`) e largura (`width`) e deve ter um `src` indicando a URL da imagem;
    - Um campo de texto pode ter `readonly`, por exemplo, para marcar que o campo não pode ser alterado. ou `required` que impede que ele seja enviado vazio.

## Estrutura básica de um documento HTML

```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Título da Página</title>
    <!-- Incluir folha de estilos CSS -->
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>Meu Site</h1>
        <nav>
            <ul>
                <li><a href="#">Página Inicial</a></li>
                <li><a href="#">Sobre</a></li>
                <li><a href="#">Contato</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section>
            <h2>Seção Principal</h2>
            <p>Conteúdo principal da página.</p>
        </section>
    </main>

    <footer>
        <p>&copy; 2024 Meu Site. Todos os direitos reservados.</p>
    </footer>
</body>
</html>

```

- `<!DOCTYPE html>` define a versão do HTML.
- `<html lang="pt-br">` define o idioma da página como português do Brasil.
- `<head>` contém metadados, como o título da página, meta tags para o charset e viewport, e links para folhas de estilo ou scripts.
- `<body>` contém todo o conteúdo visível da página, incluindo:
    - Cabeçalho (`<header>`),
    - Conteúdo principal (`<main>` com seções `<section>`), e
    - Rodapé (`<footer>`).
    

# Dev Tools

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/120b5c8b-202a-47d6-b180-84487b666423/c55f1553-6f53-4859-96bd-a025cc2a50fe/Untitled.png)

# HTML Element Reference

| Tag | Description |
| --- | --- |
| https://www.w3schools.com/tags/tag_comment.asp | Defines a comment |
| https://www.w3schools.com/tags/tag_doctype.asp | Defines the document type |
| https://www.w3schools.com/tags/tag_a.asp | Defines a hyperlink |
| https://www.w3schools.com/tags/tag_abbr.asp | Defines an abbreviation or an acronym |
| https://www.w3schools.com/tags/tag_acronym.asp | Not supported in HTML5. Use https://www.w3schools.com/tags/tag_abbr.asp instead.Defines an acronym |
| https://www.w3schools.com/tags/tag_address.asp | Defines contact information for the author/owner of a document |
| https://www.w3schools.com/tags/tag_applet.asp | Not supported in HTML5. Use https://www.w3schools.com/tags/tag_embed.asp or https://www.w3schools.com/tags/tag_object.asp instead.Defines an embedded applet |
| https://www.w3schools.com/tags/tag_area.asp | Defines an area inside an image map |
| https://www.w3schools.com/tags/tag_article.asp | Defines an article |
| https://www.w3schools.com/tags/tag_aside.asp | Defines content aside from the page content |
| https://www.w3schools.com/tags/tag_audio.asp | Defines embedded sound content |
| https://www.w3schools.com/tags/tag_b.asp | Defines bold text |
| https://www.w3schools.com/tags/tag_base.asp | Specifies the base URL/target for all relative URLs in a document |
| https://www.w3schools.com/tags/tag_basefont.asp | Not supported in HTML5. Use CSS instead.Specifies a default color, size, and font for all text in a document |
| https://www.w3schools.com/tags/tag_bdi.asp | Isolates a part of text that might be formatted in a different direction from other text outside it |
| https://www.w3schools.com/tags/tag_bdo.asp | Overrides the current text direction |
| https://www.w3schools.com/tags/tag_big.asp | Not supported in HTML5. Use CSS instead.Defines big text |
| https://www.w3schools.com/tags/tag_blockquote.asp | Defines a section that is quoted from another source |
| https://www.w3schools.com/tags/tag_body.asp | Defines the document's body |
| https://www.w3schools.com/tags/tag_br.asp | Defines a single line break |
| https://www.w3schools.com/tags/tag_button.asp | Defines a clickable button |
| https://www.w3schools.com/tags/tag_canvas.asp | Used to draw graphics, on the fly, via scripting (usually JavaScript) |
| https://www.w3schools.com/tags/tag_caption.asp | Defines a table caption |
| https://www.w3schools.com/tags/tag_center.asp | Not supported in HTML5. Use CSS instead.Defines centered text |
| https://www.w3schools.com/tags/tag_cite.asp | Defines the title of a work |
| https://www.w3schools.com/tags/tag_code.asp | Defines a piece of computer code |
| https://www.w3schools.com/tags/tag_col.asp | Specifies column properties for each column within a <colgroup> element |
| https://www.w3schools.com/tags/tag_colgroup.asp | Specifies a group of one or more columns in a table for formatting |
| https://www.w3schools.com/tags/tag_data.asp | Adds a machine-readable translation of a given content |
| https://www.w3schools.com/tags/tag_datalist.asp | Specifies a list of pre-defined options for input controls |
| https://www.w3schools.com/tags/tag_dd.asp | Defines a description/value of a term in a description list |
| https://www.w3schools.com/tags/tag_del.asp | Defines text that has been deleted from a document |
| https://www.w3schools.com/tags/tag_details.asp | Defines additional details that the user can view or hide |
| https://www.w3schools.com/tags/tag_dfn.asp | Specifies a term that is going to be defined within the content |
| https://www.w3schools.com/tags/tag_dialog.asp | Defines a dialog box or window |
| https://www.w3schools.com/tags/tag_dir.asp | Not supported in HTML5. Use https://www.w3schools.com/tags/tag_ul.asp instead.Defines a directory list |
| https://www.w3schools.com/tags/tag_div.asp | Defines a section in a document |
| https://www.w3schools.com/tags/tag_dl.asp | Defines a description list |
| https://www.w3schools.com/tags/tag_dt.asp | Defines a term/name in a description list |
| https://www.w3schools.com/tags/tag_em.asp | Defines emphasized text |
| https://www.w3schools.com/tags/tag_embed.asp | Defines a container for an external application |
| https://www.w3schools.com/tags/tag_fieldset.asp | Groups related elements in a form |
| https://www.w3schools.com/tags/tag_figcaption.asp | Defines a caption for a <figure> element |
| https://www.w3schools.com/tags/tag_figure.asp | Specifies self-contained content |
| https://www.w3schools.com/tags/tag_font.asp | Not supported in HTML5. Use CSS instead.Defines font, color, and size for text |
| https://www.w3schools.com/tags/tag_footer.asp | Defines a footer for a document or section |
| https://www.w3schools.com/tags/tag_form.asp | Defines an HTML form for user input |
| https://www.w3schools.com/tags/tag_frame.asp | Not supported in HTML5.Defines a window (a frame) in a frameset |
| https://www.w3schools.com/tags/tag_frameset.asp | Not supported in HTML5.Defines a set of frames |
| https://www.w3schools.com/tags/tag_hn.asp | Defines HTML headings |
| https://www.w3schools.com/tags/tag_head.asp | Contains metadata/information for the document |
| https://www.w3schools.com/tags/tag_header.asp | Defines a header for a document or section |
| https://www.w3schools.com/tags/tag_hgroup.asp | Defines a header and related content |
| https://www.w3schools.com/tags/tag_hr.asp | Defines a thematic change in the content |
| https://www.w3schools.com/tags/tag_html.asp | Defines the root of an HTML document |
| https://www.w3schools.com/tags/tag_i.asp | Defines a part of text in an alternate voice or mood |
| https://www.w3schools.com/tags/tag_iframe.asp | Defines an inline frame |
| https://www.w3schools.com/tags/tag_img.asp | Defines an image |
| https://www.w3schools.com/tags/tag_input.asp | Defines an input control |
| https://www.w3schools.com/tags/tag_ins.asp | Defines a text that has been inserted into a document |
| https://www.w3schools.com/tags/tag_kbd.asp | Defines keyboard input |
| https://www.w3schools.com/tags/tag_label.asp | Defines a label for an <input> element |
| https://www.w3schools.com/tags/tag_legend.asp | Defines a caption for a <fieldset> element |
| https://www.w3schools.com/tags/tag_li.asp | Defines a list item |
| https://www.w3schools.com/tags/tag_link.asp | Defines the relationship between a document and an external resource (most used to link to style sheets) |
| https://www.w3schools.com/tags/tag_main.asp | Specifies the main content of a document |
| https://www.w3schools.com/tags/tag_map.asp | Defines an image map |
| https://www.w3schools.com/tags/tag_mark.asp | Defines marked/highlighted text |
| https://www.w3schools.com/tags/tag_menu.asp | Defines an unordered list |
| https://www.w3schools.com/tags/tag_meta.asp | Defines metadata about an HTML document |
| https://www.w3schools.com/tags/tag_meter.asp | Defines a scalar measurement within a known range (a gauge) |
| https://www.w3schools.com/tags/tag_nav.asp | Defines navigation links |
| https://www.w3schools.com/tags/tag_noframes.asp | Not supported in HTML5.Defines an alternate content for users that do not support frames |
| https://www.w3schools.com/tags/tag_noscript.asp | Defines an alternate content for users that do not support client-side scripts |
| https://www.w3schools.com/tags/tag_object.asp | Defines a container for an external application |
| https://www.w3schools.com/tags/tag_ol.asp | Defines an ordered list |
| https://www.w3schools.com/tags/tag_optgroup.asp | Defines a group of related options in a drop-down list |
| https://www.w3schools.com/tags/tag_option.asp | Defines an option in a drop-down list |
| https://www.w3schools.com/tags/tag_output.asp | Defines the result of a calculation |
| https://www.w3schools.com/tags/tag_p.asp | Defines a paragraph |
| https://www.w3schools.com/tags/tag_param.asp | Defines a parameter for an object |
| https://www.w3schools.com/tags/tag_picture.asp | Defines a container for multiple image resources |
| https://www.w3schools.com/tags/tag_pre.asp | Defines preformatted text |
| https://www.w3schools.com/tags/tag_progress.asp | Represents the progress of a task |
| https://www.w3schools.com/tags/tag_q.asp | Defines a short quotation |
| https://www.w3schools.com/tags/tag_rp.asp | Defines what to show in browsers that do not support ruby annotations |
| https://www.w3schools.com/tags/tag_rt.asp | Defines an explanation/pronunciation of characters (for East Asian typography) |
| https://www.w3schools.com/tags/tag_ruby.asp | Defines a ruby annotation (for East Asian typography) |
| https://www.w3schools.com/tags/tag_s.asp | Defines text that is no longer correct |
| https://www.w3schools.com/tags/tag_samp.asp | Defines sample output from a computer program |
| https://www.w3schools.com/tags/tag_script.asp | Defines a client-side script |
| https://www.w3schools.com/tags/tag_search.asp | Defines a search section |
| https://www.w3schools.com/tags/tag_section.asp | Defines a section in a document |
| https://www.w3schools.com/tags/tag_select.asp | Defines a drop-down list |
| https://www.w3schools.com/tags/tag_small.asp | Defines smaller text |
| https://www.w3schools.com/tags/tag_source.asp | Defines multiple media resources for media elements (<video> and <audio>) |
| https://www.w3schools.com/tags/tag_span.asp | Defines a section in a document |
| https://www.w3schools.com/tags/tag_strike.asp | Not supported in HTML5. Use https://www.w3schools.com/tags/tag_del.asp or https://www.w3schools.com/tags/tag_s.asp instead.Defines strikethrough text |
| https://www.w3schools.com/tags/tag_strong.asp | Defines important text |
| https://www.w3schools.com/tags/tag_style.asp | Defines style information for a document |
| https://www.w3schools.com/tags/tag_sub.asp | Defines subscripted text |
| https://www.w3schools.com/tags/tag_summary.asp | Defines a visible heading for a <details> element |
| https://www.w3schools.com/tags/tag_sup.asp | Defines superscripted text |
| https://www.w3schools.com/tags/tag_svg.asp | Defines a container for SVG graphics |
| https://www.w3schools.com/tags/tag_table.asp | Defines a table |
| https://www.w3schools.com/tags/tag_tbody.asp | Groups the body content in a table |
| https://www.w3schools.com/tags/tag_td.asp | Defines a cell in a table |
| https://www.w3schools.com/tags/tag_template.asp | Defines a container for content that should be hidden when the page loads |
| https://www.w3schools.com/tags/tag_textarea.asp | Defines a multiline input control (text area) |
| https://www.w3schools.com/tags/tag_tfoot.asp | Groups the footer content in a table |
| https://www.w3schools.com/tags/tag_th.asp | Defines a header cell in a table |
| https://www.w3schools.com/tags/tag_thead.asp | Groups the header content in a table |
| https://www.w3schools.com/tags/tag_time.asp | Defines a specific time (or datetime) |
| https://www.w3schools.com/tags/tag_title.asp | Defines a title for the document |
| https://www.w3schools.com/tags/tag_tr.asp | Defines a row in a table |
| https://www.w3schools.com/tags/tag_track.asp | Defines text tracks for media elements (<video> and <audio>) |
| https://www.w3schools.com/tags/tag_tt.asp | Not supported in HTML5. Use CSS instead.Defines teletype text |
| https://www.w3schools.com/tags/tag_u.asp | Defines some text that is unarticulated and styled differently from normal text |
| https://www.w3schools.com/tags/tag_ul.asp | Defines an unordered list |
| https://www.w3schools.com/tags/tag_var.asp | Defines a variable |
| https://www.w3schools.com/tags/tag_video.asp | Defines embedded video content |
| https://www.w3schools.com/tags/tag_wbr.asp | Defines a possible line-break |