< FLASHFIXTECH SOLUTIONS>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Flashfix Tech Solutions</title>
  <style>
    /* ===== RESET ===== */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: "Poppins", sans-serif;
      background: #f4f8ff;
      color: #333;
      line-height: 1.6;
      scroll-behavior: smooth;
    }

    header {
      background: linear-gradient(135deg, #007bff, #00c6ff);
      color: white;
      text-align: center;
      padding: 80px 20px;
    }

    header h1 {
      font-size: 2.5rem;
      margin-bottom: 10px;
    }

    header p {
      font-size: 1.1rem;
      margin-bottom: 20px;
    }

    .btn {
      background: white;
      color: #007bff;
      padding: 12px 25px;
      border-radius: 30px;
      text-decoration: none;
      font-weight: bold;
      transition: 0.3s;
    }

    .btn:hover {
      background: #e6e6e6;
    }

    /* ===== SERVICES ===== */
    section {
      padding: 60px 20px;
      text-align: center;
    }

    h2 {
      color: #007bff;
      font-size: 2rem;
      margin-bottom: 30px;
    }

    .services {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
      max-width: 1000px;
      margin: 0 auto;
    }

    .service {
      background: white;
      padding: 25px;
      border-radius: 15px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
      transition: transform 0.3s ease;
    }

    .service:hover {
      transform: translateY(-5px);
    }

    .service h3 {
      color: #007bff;
      margin-bottom: 10px;
    }

    /* ===== GALLERY ===== */
    .gallery {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 10px;
      max-width: 900px;
      margin: 0 auto;
    }

    .gallery img {
      width: 100%;
      border-radius: 10px;
      height: 180px;
      object-fit: cover;
    }

    /* ===== CONTACT ===== */
    footer {
      background: #222;
      color: white;
      text-align: center;
      padding: 40px 20px;
    }

    footer h3 {
      color: #00c6ff;
      margin-bottom: 10px;
    }

    footer p {
      margin: 5px 0;
    }

    footer a {
      color: #00c6ff;
      text-decoration: none;
    }

    footer a:hover {
      text-decoration: underline;
    }

    /* ===== MOBILE ===== */
    @media (max-width: 768px) {
      header h1 {
        font-size: 2rem;
      }
      .btn {
        padding: 10px 20px;
      }
    }
  </style>
</head>
<body>
  <header>
    <h1>Welcome to Flashfix Tech Solutions</h1>
    <p>We bring your ideas to life with technology, creativity, and precision.</p>
    <a href="#contact" class="btn">Contact Us</a>
  </header>

  <section id="services">
    <h2>Our Services</h2>
    <div class="services">
      <div class="service">
        <h3>Website Design</h3>
        <p>Modern, responsive websites that convert visitors into customers.</p>
      </div>
      <div class="service">
        <h3>Graphic Design</h3>
        <p>Professional posters, logos, and social media designs.</p>
      </div>
      <div class="service">
        <h3>Video Editing</h3>
        <p>Engaging, cinematic edits for your brand, ads, or content.</p>
      </div>
      <div class="service">
        <h3>Tech Repairs</h3>
        <p>Reliable gadget repairs and system maintenance solutions.</p>
      </div>
      <div class="service">
        <h3>Digital Marketing</h3>
        <p>Grow your online presence and attract more clients with smart strategies.</p>
      </div>
      <div class="service">
        <h3>IT Consultancy</h3>
        <p>Expert guidance on digital transformation and tech solutions.</p>
      </div>
    </div>
  </section>

  <section id="gallery">
    <h2>Our Work</h2>
    <div class="gallery">
      <img src="https://source.unsplash.com/400x300/?webdesign" alt="Website Design">
      <img src="https://source.unsplash.com/400x300/?graphic,design" alt="Graphic Design">
      <img src="https://source.unsplash.com/400x300/?video,editing" alt="Video Editing">
      <img src="https://source.unsplash.com/400x300/?computer,repair" alt="Tech Repairs">
    </div>
  </section>

  <footer id="contact">
    <h3>Contact Us</h3>
    <p>Phone: <a href="tel:0705305516">0705305516</a></p>
    <p>Email: <a href="mailto:flashfixedits@gmail.com">flashfixedits@gmail.com</a></p>
    <p>&copy; 2025 Flashfix Tech Solutions. All Rights Reserved.</p>
  </footer>

  <script>
    // Simple scroll alert
    document.querySelector('.btn').addEventListener('click', () => {
      alert('Thanks for reaching out to Flashfix Tech Solutions!');
    });
  </script>
</body>
</html>
update index 
‎<!-- IMAGE UPLOAD + PREVIEW (Drop this where you want the upload tools) -->
‎<section id="upload-photos" style="padding:30px;text-align:center;max-width:900px;margin:0 auto;">
‎  <h2>Upload up to 4 photos</h2>
‎
‎  <p style="margin:8px 0 16px;color:#555;">Select up to <strong>4</strong> images (jpg/png). Previews will appear below.</p>
‎
‎  <input id="imageInput" type="file" accept="image/*" multiple />
‎  <div style="margin-top:12px;">
‎    <button id="addToGalleryBtn" class="btn" style="background:#007bff;color:white;border:none;padding:10px 16px;border-radius:8px;cursor:pointer;">Add to Gallery</button>
‎  </div>
‎
‎  <div id="previewContainer" style="display:grid;grid-template-columns:repeat(auto-fit,minmax(140px,1fr));gap:12px;margin-top:18px;"></div>
‎  <p id="uploadMsg" style="color:#b00;margin-top:8px;"></p>
‎</section>
‎
‎<!-- EXAMPLE GALLERY SECTION (where images will be inserted) -->
‎<section id="liveGallery" style="padding:30px;text-align:center;">
‎  <h2>Our Work (Live Gallery)</h2>
‎  <div id="galleryGrid" style="display:grid;grid-template-columns:repeat(auto-fit,minmax(200px,1fr));gap:10px;max-width:900px;margin:12px auto;"></div>
‎</section>
‎
‎<script>
‎  // LIMIT: max 4 files
‎  const MAX_FILES = 4;
‎  const imageInput = document.getElementById('imageInput');
‎  const previewContainer = document.getElementById('previewContainer');
‎  const addToGalleryBtn = document.getElementById('addToGalleryBtn');
‎  const uploadMsg = document.getElementById('uploadMsg');
‎  const galleryGrid = document.getElementById('galleryGrid');
‎
‎  let chosenFiles = []; // File objects chosen in current selection
‎
‎  imageInput.addEventListener('change', (e) => {
‎    previewContainer.innerHTML = '';
‎    uploadMsg.textContent = '';
‎    chosenFiles = Array.from(e.target.files || []);
‎
‎    if (chosenFiles.length === 0) return;
‎
‎    if (chosenFiles.length > MAX_FILES) {
‎      uploadMsg.textContent = `Please select at most ${MAX_FILES} images. You selected ${chosenFiles.length}.`;
‎      chosenFiles = chosenFiles.slice(0, MAX_FILES);
‎    }
‎
‎    // Preview each file
‎    chosenFiles.forEach((file, idx) => {
‎      if (!file.type.startsWith('image/')) return; // skip non-images
‎
‎      const reader = new FileReader();
‎      const wrapper = document.createElement('div');
‎      wrapper.style = "position:relative;border-radius:8px;overflow:hidden;background:#fff;padding:6px;box-shadow:0 2px 6px rgba(0,0,0,0.08);";
‎
‎      const removeBtn = document.createElement('button');
‎      removeBtn.textContent = '×';
‎      removeBtn.title = 'Remove';
‎      removeBtn.style = 'position:absolute;top:6px;right:6px;background:#0008;color:white;border:none;border-radius:50%;width:26px;height:26px;cursor:pointer;z-index:3';
‎
‎      removeBtn.addEventListener('click', () => {
‎        // remove this file from chosenFiles
‎        chosenFiles.splice(idx, 1);
‎        // update input.files by creating a new DataTransfer
‎        const dt = new DataTransfer();
‎        chosenFiles.forEach(f => dt.items.add(f));
‎        imageInput.files = dt.files;
‎        wrapper.remove();
‎      });
‎
‎      const img = document.createElement('img');
‎      img.style = 'width:100%;height:140px;object-fit:cover;border-radius:6px;display:block;';
‎
‎      reader.onload = (ev) => {
‎        img.src = ev.target.result;
‎      };
‎      reader.readAsDataURL(file);
‎
‎      wrapper.appendChild(removeBtn);
‎      wrapper.appendChild(img);
‎      previewContainer.appendChild(wrapper);
‎    });
‎  });
‎
‎  // When user clicks "Add to Gallery" we insert previews into the live gallery
‎  addToGalleryBtn.addEventListener('click', (e) => {
‎    e.preventDefault();
‎    uploadMsg.textContent = '';
‎
‎    if (chosenFiles.length === 0) {
‎      uploadMsg.textContent = 'No images selected. Please choose up to 4 images first.';
‎      return;
‎    }
‎
‎    // Insert each selected image into the live gallery (client-side only)
‎    chosenFiles.forEach(file => {
‎      if (!file.type.startsWith('image/')) return;
‎      const reader = new FileReader();
‎      reader.onload = (ev) => {
‎        const imgWrap = document.createElement('div');
‎        imgWrap.style = 'background:#fff;border-radius:10px;overflow:hidden;box-shadow:0 4px 10px rgba(0,0,0,0.06);';
‎        const img = document.createElement('img');
‎        img.src = ev.target.result;
‎        img.alt = file.name;
‎        img.style = 'width:100%;height:170px;object-fit:cover;display:block;';
‎        imgWrap.appendChild(img);
‎        galleryGrid.appendChild(imgWrap);
‎      };
‎      reader.readAsDataURL(file);
‎    });
‎
‎    // Clear selection and previews after adding
‎    imageInput.value = '';
‎    previewContainer.innerHTML = '';
‎    chosenFiles = [];
‎    uploadMsg.style.color = '#090';
‎    uploadMsg.textContent = 'Images added to gallery (temporary, client-side). To save permanently, upload files to your repository.';
‎    setTimeout(()=>{ uploadMsg.textContent = ''; uploadMsg.style.color = '#b00'; }, 5000);
‎  });
‎</script>
‎
