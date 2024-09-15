---
layout: single 
permalink: /fields/
author_profile: false
author: Lila Chamlagai
title: "Field Work"
toc: false
header:
  overlay_color: "#000"
  overlay_image: /assets/images/field.jpg
---

<div class="gallery-container">
    <div class="gallery" id="gallery">
        <div class="slide">
            <img src="/assets/images/fig1.JPG" alt="Data Collection In Nepal Refugee Camp">
            <div class="caption">Data Collection In Nepal Refugee Camp</div>
        </div>
        <div class="slide">
            <img src="/assets/images/fig2.JPG" alt="Impact of Drugs and Gangsters on Mental Health in Brazil">
            <div class="caption">Impact of Drugs and Gangsters on Mental Health in Brazil</div>
        </div>
        <div class="slide">
            <img src="/assets/images/fig3.JPG" alt="South Africa Travelling -- HIVAIDS Ethnographic Data Collection">
            <div class="caption">South Africa Travelling -- HIVAIDS Ethnographic Data Collection</div>
        </div>
        <div class="slide">
            <img src="/assets/images/fig4.JPG" alt="Communicating with Xhan-- Hunter-gatherer at Kalahari Desert">
            <div class="caption">Communicating with Xhan-- Hunter-gatherer at Kalahari Desert</div>
        </div>
        <div class="slide">
            <img src="/assets/images/fig5.JPG" alt="Awareness about the HIV-AIDS in South Africa">
            <div class="caption">Awareness about the HIV-AIDS in South Africa</div>
        </div>
        <div class="slide">
            <img src="/assets/images/fig6.JPG" alt="Volunteering at School in South Africa">
            <div class="caption">Volunteering at School in South Africa</div>
        </div>
    </div>
</div>

<style>
    body {
        font-family: Arial, sans-serif;
        margin: 0;
        padding: 0;
        overflow: hidden;
    }
    .gallery-container {
        position: relative;
        height: 100vh;
        display: flex;
        align-items: center;
        justify-content: center;
        overflow: hidden;
    }
    .gallery {
        position: absolute;
        width: 100%;
        height: 100%;
        display: flex;
        transition: transform 1s ease-in-out;
    }
    .gallery img {
        width: 100%;
        height: auto;
        display: block;
    }
    .caption {
        position: absolute;
        top: 10%;
        left: 50%;
        transform: translateX(-50%);
        color: white;
        text-shadow: 0 0 10px rgba(0, 0, 0, 0.7);
        font-size: 24px;
        text-align: center;
    }
    @media (max-width: 600px) {
        .caption {
            font-size: 18px;
        }
    }
</style>

<script>
    const gallery = document.getElementById('gallery');
    let index = 0;

    function showNextSlide() {
        index = (index + 1) % gallery.children.length;
        gallery.style.transform = `translateX(-${index * 100}%)`;
    }

    setInterval(showNextSlide, 3000); // Change slide every 3 seconds
</script>
