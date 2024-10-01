<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles.css">
    <title>Chillz Entertainment Company</title>
</head>
<body><section id="slideshow"></section>
    <h2>Experience the Fun!</h2>
    <div class="slideshow-container">
        <div class="mySlides fade">
            <img src="Screenshot_20241001_034523_Chrome.jpg" style="width:100%">
            <div class="text">Amazing Party Atmosphere</div>
        </div>

        <div class="mySlides fade">
            <img src="IMG_20240815_113649_100.jpg" style="width:100%">
            <div class="text">Dance the Night Away</div>
        </div>

        <div class="mySlides fade">
            <img src="IMG-20240926-WA0003.jpg" style="width:100%">
            <div class="text">Unforgettable Memories</div>
        </div>

        <div class="navigation">
            <a class="prev" onclick="plusSlides(-1)">&#10094;</a>
            <a class="next" onclick="plusSlides(1)">&#10095;</a>
        </div>
    </div>
</section>

<script>
    let slideIndex = 0;
    showSlides();

    function showSlides() {
        let i;
        const slides = document.getElementsByClassName("mySlides");
        for (i = 0; i < slides.length; i++) {
            slides[i].style.display = "none";  
        }
        slideIndex++;
        if (slideIndex > slides.length) {slideIndex = 1}    
        for (i = 0; i < slides.length; i++) {
            slides[i].style.display = "none";  
        }
        slides[slideIndex-1].style.display = "block";  
        setTimeout(showSlides, 3000); // Change image every 3 seconds
    }

    function plusSlides(n) {
        slideIndex += n;
        if (slideIndex > slides.length) {slideIndex = 1}
        if (slideIndex < 1) {slideIndex = slides.length}    
        showSlides();
    }
</script>
    <header>
        <h1>Welcome to Chillz Entertainment</h1>
        <p>Chillz to the People, Chillz to the Nation</p>
    </header>
    <nav>
        <ul>
            <li><a href="#about">About Us</a></li>
            <li><a href="#services">Our Services</a></li>
            <li><a href="#contact">Contact Us</a></li>
        </ul>
    </nav>
    <section id="about">
        <h2>About Us</h2>
        <p>At Chillz Entertainment, we specialize in creating unforgettable experiences. Whether it's a birthday party, corporate event, or community gathering, our mission is to bring joy and excitement!</p>
    </section>
    <section id="services">
        <h2>Our Services</h2>
        <ul>
            <li>Event Planning</li>
            <li>Live DJ Performances</li>
            <li>Party Games and Activities</li>
            <li>Lighting and Sound Systems</li>
        </ul>
        <p>We ensure that every event is filled with fun and laughter, making your gatherings memorable!</p>
    </section>
    <section id="testimonials">
        <h2>What Our Clients Say</h2>
        <blockquote>"Chillz Entertainment turned our party into something magical! Everyone had a blast!" - Sarah T.</blockquote>
        <blockquote>"The DJ was incredible and kept the dance floor full all night!" - Mike G.</blockquote>
    </section>
    <section id="contact">
        <h2>Contact Us</h2>
        <p>Ready to plan your next event? Get in touch!</p>
        <form>
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" required>
            
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>
            
            <label for="message">Message:</label>
            <textarea id="message" name="message" required></textarea>
            
            <button type="submit">Send Message</button>
        </form>
    </section>
    <footer>
        <p>&copy; 2023 Chillz Entertainment. All Rights Reserved.</p>
    </footer>
</body>
</html>
