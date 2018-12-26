# partner-module

## Prerequisites
<ul>
	<li><a target="_blank" href="https://getbootstrap.com/">Boostrap4</a></li>
	<li><a target="_blank" href="https://fontawesome.com/">FontAwesome5</a></li>
</ul>

## Step 1: Add the Form
 - partner-form.tpl

Create a calendar for the Partners and upload the following form. Be sure to replace SITE_NAME with your site's name.

```
<div class="panel-group">
  <div class="panel panel-default">
    <div class="panel-heading">
      <h4 class="panel-title"><a aria-expanded="true" data-toggle="collapse" href="#collapseStatus">Post Status<span
            class="toggle" aria-hidden="true"></span></a></h4>
    </div>

    <div class="panel-collapse collapse in" id="collapseStatus">
      <div class="panel-body">
        <div class="row">
          <div class="col-md-3">
            <h2><label class="label-control" for="post_status">Post Status</label></h2>
            <select class="form-control" name="post_status" type="text">
              <option value="Draft">Draft</option>
              <option value="Published">Published</option>
            </select>
          </div>

          <div class="col-md-3">
            <h2><label class="label-control" for="post_author">Post Author</label></h2>
            <select class="form-control" name="post_author" type="text">
              <option value="None">None</option>
              <option value="AUTHOR_NAME">AUTHOR_NAME</option>
            </select>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

<div class="panel-group">
  <div class="panel panel-default">
    <div class="panel-heading">
      <h4 class="panel-title"><a aria-expanded="true" data-toggle="collapse" href="#collapseInfo">Client Info <span
            class="toggle" aria-hidden="true"></span></a></h4>
    </div>

    <div class="panel-collapse collapse in" id="collapseInfo">
      <div class="panel-body">
        <div class="row">


          <div class="col-md-4">
            <h2><label class="label-control" for="featured_client_image">Featured Image</label></h2>
            <input class="file_upload" id="featured_client_image" name="featured_client_image" required="" type="file" />
          </div>

          <div class="col-md-4">
            <h2><label class="label-control" for="featured_detail_image">Detail Image</label></h2>
            <input class="file_upload" id="featured_detail_image" name="featured_detail_image" required="" type="file" />
          </div>

          <div class="col-md-4">
            <h2><label class="label-control" for="client_url">Client Website URL</label></h2>
            <input class="form-control" id="client_url" name="client_url" required="" type="text" />
          </div>
        </div>


      </div>
    </div>
  </div>
</div>

<div class="panel-group">
  <div class="panel panel-default">
    <div class="panel-heading">
      <h4 class="panel-title"><a aria-expanded="true" data-toggle="collapse" href="#collapseContent">Post Content<span
            class="toggle" aria-hidden="true"></span></a></h4>
    </div>

    <div class="panel-collapse collapse in" id="collapseContent">
      <div class="panel-body">
        <div class="row">
          <div class="col-md-12">
            <h2><label class="label-control" for="heading_title">Heading Overwrite</label></h2>

            <p class="subText">(Optional) If specified, this will overwrite the article's title and become the main
              heading.</p>
            <input class="form-control" id="heading_title" name="heading_title" type="text" />
          </div>
        </div>

        <div class="row">
          <div class="col-md-12">
            <h2><label class="label-control" for="post_intro">Intro/Subtitle</label></h2>

            <p class="subText">(Required) Content that appears before the Body Content and the introductory paragraph
              on the blogroll.</p>
            <textarea class="form-control" id="post_intro" name="post_intro" required=""></textarea>
          </div>
        </div>

        <div class="row">
          <div class="col-md-12">
            <h2><label class="label-control" for="post_content">Body Content</label></h2>

            <p class="subText">(Required) The main content section for an article.</p>
            <textarea class="wysiwyg" id="post_content" name="post_content" required=""></textarea>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

<div class="panel-group">
  <div class="panel panel-default">
    <div class="panel-heading">
      <h4 class="panel-title"><a data-toggle="collapse" href="#collapseMeta">META Data <span class="toggle" aria-hidden="true"></span></a></h4>
    </div>

    <div class="panel-collapse collapse" id="collapseMeta">
      <div class="panel-body">
        <div class="row">
          <div class="col-md-12">
            <h2><label name="meta_title">Meta Title</label></h2>

            <p class="subText">(Optional) Include a custom META Title that will show in your browser tab and in the
              page's source code.</p>
            <input class="form-control" id="meta_title" name="meta_title" type="text" />
          </div>
        </div>

        <div class="row">
          <div class="col-md-12">
            <h2><label name="meta_description">Meta Description</label></h2>

            <p class="subText">(Optional) Include a custom META Description that search engines will index. 50-160
              Characters</p>
            <textarea class="form-control" id="meta_description" name="meta_description"></textarea>
          </div>
        </div>

        <div class="row">
          <div class="col-md-12">
            <h2><label name="meta_keywords">Meta Keywords</label></h2>

            <p class="subText">(Optional) Include the main keywords of the blog article.</p>
            <textarea class="form-control" id="meta_keywords" name="meta_keywords"></textarea>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

<div class="panel-group">
  <div class="panel panel-default">
    <div class="panel-heading">
      <h4 class="panel-title"><a data-toggle="collapse" href="#collapseAdvanced">Advanced <span class="toggle"
            aria-hidden="true"></span></a></h4>
    </div>

    <div class="panel-collapse collapse" id="collapseAdvanced">
      <div class="panel-body">
        <div class="row">
          <div class="col-md-12">
            <h2><label class="label-control" for="post_javascript">Custom JavaScript</label></h2>

            <p class="subText">(Optional) Use the following textbox to embed any custom JavaScript including tracking
              pixels and Google Analytics scripts. Be sure to open your JavaScript with a &lt;script&gt; tag and close
              everything with a &lt;/script&gt; tag.</p>
            <textarea class="form-control" id="post_javascript" name="post_javascript"></textarea>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>
<?php
            if(isset($dataVars['calendar_entry_id'])){     
              $calendar_entry = new Calendar_Entry($dataVars['calendar_entry_id']);
              if($calendar_entry->path) { 
          ?>

<div class="panel-group">
  <div class="panel panel-default">
    <div class="panel-heading">
      <h4 class="panel-title"><a data-toggle="collapse" href="#collapseURL">Post URL <span class="toggle" aria-hidden="true"></span></a></h4>
    </div>

    <div class="panel-collapse collapse in" id="collapseURL">
      <div class="panel-body">
        <div class="row">
          <div class="col-md-12">
            <p class="subText">You can access this blog post at the following URL:</p>
            <a href="http://www.SITE_NAME.com<?= $calendar_entry->path ?>" target="_blank">http://www.SITE_NAME.com<?= $calendar_entry->path ?></a>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>
<?php 
              } 
            }
           ?>
<script>
  $('.wysiwyg').ckeditor(function () {}, {
    customConfig: '/CK/config.js',
    height: '600px',
    basePath: '/CK/',
    toolbar: 'WP'
  });
</script>

```

## Step 2: Add the Repeater
 - partner-repeater.tpl

Add the following repeater shortcode. 

```
<div class="row">
[repeater id='3'  pages="22" order="start_time desc" display_type="news" where="post_status='Published'"]
  <div class="col-md-4 p-0 h-225p d-flex">
    <a href="{{path}}" class="text-center d-block w-100 h-100 d-flex align-items-center justify-content-center">
      <img class="p-md-3 p-lg-4 img-fluid" alt="{{event_title}}" src="[get_asset_file_url id={{featured_client_image}}]">
    </a>
  </div>
[/repeater]
</div>
```

## Step 3: Add the Detail Template
- partner-detail.tpl

```
[entry]
  <div class="text-center">
    <p class="lead">{{post_intro}}</p>
  </div>
  <img alt="{{heading_title}}" class="w-100 img-fluid my-4" src="[get_asset_file_url id={{featured_detail_image}}]"></div>

  <div class="row mt-5 px-5">
    <div class="col-lg-8">
      [is_set value={{heading_title}}]
       <h2 class="mb-5"><strong>{{heading_title}}</strong></h2>
      [/is_set]
      [is_empty value={{heading_title}}]
       <h2 class="mb-5"><strong>{{event_title}}</strong></h2>
      [/is_empty]
      {{post_content}}
      <div class="text-center mt-5">
        <a href="{{client_url}}" class="btn btn-lg btn-outline-secondary" target="blank">Launch Site</a>
      </div>
    </div>
    <div class="col-lg-3 ml-auto d-md-none d-lg-block">
      <ul class="list-unstyled d-flex align-items-center pb-3">
        <li class="lead mr-2 my-0"><strong>Share</strong></li>
        <li class="mb-0"><a href="#" class="text-secondary" target="_blank"><i class="pl-3 text-hover-primary fa-lg fab fa-facebook-f"></i></a></li>
        <li class="mb-0"><a href="#" class="text-secondary" target="_blank"><i class="pl-3 text-hover-primary fa-lg fab fa-twitter"></i></a></li>
        <li class="mb-0"><a href="#" class="text-secondary" target="_blank"><i class="pl-3 text-hover-primary fa-lg fab fa-linkedin-in"></i></a></li>
      </ul>
      <h3 class="border-top pt-3">Services Included</h3>
      <ul class="list-unstyled">
        [entry_categories_repeat id="{{calendar_entry_id}}"]
            <li>{{{title}}}</li>
          [/entry_categories_repeat]
      </ul>
    </div>
  </div>
[/entry]

```

## Step 4: Add the SCSS/SCC
  - /_/scss/partner.scss

```
.h-225p {
    height: 225px;
}

.btn-outline-secondary {
    color: #3d5d6f;
    background-color: transparent;
    background-image: none;
    border-color: #3d5d6f;
}

.text-hover-primary {
    &:hover {
        color: #d60e96 !important;
    }
}

```
