<style>
.gallery-container {
  width: 100%;
  position: relative;
  overflow: hidden;
}
.gallery-frame {
  position: relative;
  width: 100%;
  padding-top: 56.25%; /* Tỷ lệ 16:9 */
  border: 1px solid #ddd;
  overflow: visible; /* Cho phép nội dung tràn ra ngoài */
}
.gallery-images {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  display: flex;
  justify-content: center;
}
.gallery-item {
  position: relative;
  height: 100%;
  flex: 1;
  transition: all 0.4s ease;
  overflow: hidden;
  min-width: 0; /* Cho phép item co lại nhỏ hơn nội dung */
}
.gallery-item:hover {
  flex: 0 0 100%; /* Chiếm toàn bộ chiều rộng khi hover */
  z-index: 1;
}
.gallery-images:hover .gallery-item:not(:hover) {
  flex: 0 0 0; /* Thu nhỏ hoàn toàn các ảnh khác */
  opacity: 0;
}
.gallery-item img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  transition: transform 0.4s ease;
}
.gallery-item:hover img {
  transform: scale(1.05);
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