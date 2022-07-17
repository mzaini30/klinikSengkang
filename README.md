# Klinik Sengkang

Dokumentasi template Klinik Sengkang

## Mengedit Slider

Untuk mengedit Slider, buka halaman beranda Klinik Sengkang. Lalu, klik "Sunting dengan Elementor". Kemudian, edit bagian slider. Maka, kamu akan mendapatkan kode seperti di bawah ini:

```html
<img src="" alt="" class="sliderSimpel" />
<script>
  let angkaSlider = 0;
  function sliderSimpel() {
    const list = [
      "//kliniksengkang.id/wp-content/uploads/2022/06/apotek-sengkang-1-scaled-1.webp",
      "//kliniksengkang.id/wp-content/uploads/2022/06/apotek-sengkang-2-scaled-1.webp",
      "//kliniksengkang.id/wp-content/uploads/2022/06/apotek-sengkang-3-scaled-1.webp",
      "//kliniksengkang.id/wp-content/uploads/2022/06/apotek-sengkang-4-scaled-1.webp",
    ];
    const elSlider = document.querySelector(".sliderSimpel");
    elSlider.src = list[angkaSlider % list.length];
    angkaSlider++;
  }
  sliderSimpel();
  setInterval(sliderSimpel, 1000 * 60);
</script>
<style>
  .sliderSimpel {
    width: 100vw !important;
    max-width: 100vw !important;
    height: auto;
    margin-left: -5%;
  }
  @media (min-width: 674px) {
    .sliderSimpel {
      margin-left: -4%;
    }
  }
  @media (min-width: 814px) {
    .sliderSimpel {
      margin-left: -3%;
    }
  }
  @media (min-width: 881px) {
    .sliderSimpel {
      margin-left: -4%;
    }
  }
  @media (min-width: 1025px) {
    .sliderSimpel {
      margin-left: -8%;
    }
  }
  @media (min-width: 1100px) {
    .sliderSimpel {
      margin-left: -6%;
    }
  }
</style>
```

Maka, list gambarnya itu adalah sekumpulan link gambar yang terletak di bawahnya `const list = [`. Untuk formatnya, harus diapit oleh kutip dan diakhiri dengan koma (contoh: `"//kliniksengkang.id/wp-content/uploads/2022/06/apotek-sengkang-1-scaled-1.webp",`).

<!-- blog start -->
## Blog

- [Script Golang untuk Ngecek Error](https://github.zenia.my.id/tulisan/error)
- [Otomatis "go fmt" Setiap Save](https://github.zenia.my.id/tulisan/gofmt)
- [Install Workflow Automa dari Digimart](https://github.zenia.my.id/tulisan/digimart)
- [Mengatasi Bun Error Illegal Instruction](https://github.zenia.my.id/tulisan/bun)
- [Cara Enkripsi File](https://github.zenia.my.id/tulisan/enkripsi)
<!-- blog end -->
