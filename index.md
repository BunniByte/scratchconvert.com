---
layout: default
title: ScratchConvert - Convert Scratch Projects to .exe For Free!
description: All about how to convert Scratch Projects to Windows Programs, HTML5, and even Mobile Apps completely for free!
thumbnail: public/img/branding/thumbnail.png
permalink: /
---

<div class="page-header header-filter header-small" data-parallax="true" style="background-image: url('public/img/misc/header.jpg');">
    <div class="container">
        <div class="row">
            <div class="col-md-8 ml-auto mr-auto text-center">
                <h1 class="title">ScratchConvert</h1>
                <br />
            </div>
        </div>
    </div>
</div>
<div class="main main-raised">
    <div class="container">
        <div class="section section-text">
            <!-- Popular articles start -->
            <div class="row">
                <h3 class="title">Popular Articles</h3>
                            
                <div class="row">
                    <div class="col-md-6">
                        <div class="card card-raised card-background" style="background-image: url('../assets/img/examples/office2.jpg');">
                            <div class="card-body">
                                <h6 class="card-category text-info">Worlds</h6>
                                <a href="#pablo">
                                    <h3 class="card-title">The Best Productivity Apps on Market</h3>
                                </a>
                                <p class="card-description">
                                    Don't be scared of the truth because we need to restart the human foundation in truth And I love you like Kanye loves Kanye I love Rick Owens' bed design but the back is...
                                </p>
                                <a href="#pablo" class="btn btn-danger btn-round">
                                    <i class="material-icons">format_align_left</i> Read Article
                                    <div class="ripple-container"></div>
                                </a>
                            </div>
                        </div>
                    </div>
                    <div class="col-md-6">
                        <div class="card card-raised card-background" style="background-image: url('../assets/img/examples/blog8.jpg');">
                            <div class="card-body">
                                <h6 class="card-category text-info">Business</h6>
                                <h3 class="card-title">Working on Wallstreet is Not So Easy</h3>
                                <p class="card-description">
                                    Don't be scared of the truth because we need to restart the human foundation in truth And I love you like Kanye loves Kanye I love Rick Owens' bed design but the back is...
                                </p>
                                <a href="#pablo" class="btn btn-primary btn-round"> <i class="material-icons">format_align_left</i> Read Article </a>
                            </div>
                        </div>
                    </div>
                    <div class="col-md-12">
                        <div class="card card-raised card-background" style="background-image: url('../assets/img/examples/card-project6.jpg');">
                            <div class="card-body">
                                <h6 class="card-category text-info">Marketing</h6>
                                <h3 class="card-title">0 to 100.000 Customers in 6 months</h3>
                                <p class="card-description">
                                    Don't be scared of the truth because we need to restart the human foundation in truth And I love you like Kanye loves Kanye I love Rick Owens' bed design but the back is...
                                </p>
                                <a href="#pablo" class="btn btn-warning btn-round"> <i class="material-icons">subject</i> Read Case Study </a>
                                <a href="#pablo" class="btn btn-white btn-just-icon btn-link" title="" rel="tooltip" data-original-title="Save to Pocket">
                                    <i class="fab fa-get-pocket"></i>
                                    <div class="ripple-container"></div>
                                </a>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <!-- Popular articles end -->

            <!-- All articles start -->
            <div class="row">
                <h3 class="title">All Articles</h3>
                        
                <div class="row">
                    {% for post in site.posts %}
                        {% if post.isFeatured != true %}
                            <div class="col-md-4">
                                <div class="card card-blog">
                                    <div class="card-header card-header-image">
                                        <a href="https://scratchconvert.com{{ post.permalink }}">
                                            <img src="{{ post.thumbnail | default: site.thumbnail }}" alt="{{ post.title }}" />
                                        </a>
                                        <div class="colored-shadow" style="background-image: url('{{ post.thumbnail | default: site.thumbnail }}'); opacity: 1;"></div>
                                    </div>
                                    <div class="card-body">
                                        <h6 class="card-category text-warning">{{ post.category }}</h6>

                                        <h4 class="card-title">
                                            <a href="https://scratchconvert.com{{ post.permalink }}">{{ post.title }}</a>
                                        </h4>

                                        <a href="https://scratchconvert.com{{ post.permalink }}" class="btn btn-warning btn-round"> <i class="material-icons">subject</i> Read Article <div class="ripple-container"></div></a>
                                    </div>
                                </div>
                            </div>
                        {% endif %}
                    {% endfor %}
                </div>
            </div>
            <!-- All articles end -->
        </div>
    </div>
</div>