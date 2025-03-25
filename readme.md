# Image Gallery Demo

Welcome to my image gallery demo! This project showcases a responsive image gallery with hover effects.

**[View Live Demo on GitHub Pages](https://caoquocviet.github.io/github_page_img/)**

<style>
.gallery-container {
  width: 80%;
  max-width: 1200px;
  margin: 0 auto;
  position: relative;
  overflow: hidden;
  padding: 20px;
  background: #f8f9fa;
  border-radius: 15px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

.gallery-frame {
  position: relative;
  width: 100%;
  padding-top: 56.25%; /* Tỷ lệ 16:9 */
  border: 2px solid #e9ecef;
  border-radius: 12px;
  overflow: visible;
  background: white;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.05);
}

.gallery-images {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  display: flex;
  justify-content: center;
  gap: 2px;
  padding: 2px;
}

.gallery-item {
  position: relative;
  height: 100%;
  flex: 1;
  transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
  overflow: hidden;
  min-width: 0;
  border-radius: 8px;
  border: 2px solid #fff;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.gallery-item:hover {
  flex: 0 0 100%;
  z-index: 1;
  border-radius: 12px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
}

.gallery-images:hover .gallery-item:not(:hover) {
  flex: 0 0 0;
  opacity: 0;
}

.gallery-item img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  transition: transform 0.4s cubic-bezier(0.4, 0, 0.2, 1);
}

.gallery-item:hover img {
  transform: scale(1.05);
}

@media (max-width: 768px) {
  .gallery-container {
    width: 95%;
    padding: 10px;
  }
  
  .gallery-frame {
    border-radius: 8px;
  }
  
  .gallery-item {
    border-radius: 6px;
  }
  
  .gallery-item:hover {
    border-radius: 8px;
  }
}
</style>

<div class="gallery-container">
  <div class="gallery-frame">
    <div class="gallery-images">
      <div class="gallery-item">
        <img src="https://raw.githubusercontent.com/CaoQuocViet/github_page_img/main/readme/Screenshot%202025-03-02%20202830.png" alt="Ảnh 1">
      </div>
      <div class="gallery-item">
        <img src="https://raw.githubusercontent.com/CaoQuocViet/github_page_img/main/readme/Screenshot%202025-03-10%20174731.png" alt="Ảnh 2">
      </div>
      <div class="gallery-item">
        <img src="https://raw.githubusercontent.com/CaoQuocViet/github_page_img/main/readme/Screenshot%202025-03-10%20180700.png" alt="Ảnh 3">
      </div>
      <div class="gallery-item">
        <img src="https://raw.githubusercontent.com/CaoQuocViet/github_page_img/main/readme/Screenshot%202025-03-10%20214807.png" alt="Ảnh 4">
      </div>
      <div class="gallery-item">
        <img src="https://raw.githubusercontent.com/CaoQuocViet/github_page_img/main/readme/Screenshot%202025-03-10%20222222.png" alt="Ảnh 5">
      </div>
      <div class="gallery-item">
        <img src="https://raw.githubusercontent.com/CaoQuocViet/github_page_img/main/readme/Screenshot%202025-03-02%20202830.png" alt="Ảnh 6">
      </div>
      <div class="gallery-item">
        <img src="https://raw.githubusercontent.com/CaoQuocViet/github_page_img/main/readme/Screenshot%202025-03-10%20174731.png" alt="Ảnh 7">
      </div>
      <div class="gallery-item">
        <img src="https://raw.githubusercontent.com/CaoQuocViet/github_page_img/main/readme/Screenshot%202025-03-10%20180700.png" alt="Ảnh 8">
      </div>
      <div class="gallery-item">
        <img src="https://raw.githubusercontent.com/CaoQuocViet/github_page_img/main/readme/Screenshot%202025-03-10%20214807.png" alt="Ảnh 9">
      </div>
      <div class="gallery-item">
        <img src="https://raw.githubusercontent.com/CaoQuocViet/github_page_img/main/readme/Screenshot%202025-03-10%20222222.png" alt="Ảnh 10">
      </div>
    </div>
  </div>
</div>