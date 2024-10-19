<script setup>
import {ref, onMounted} from 'vue'

defineProps({
  msg: String,
})

const count = ref(0)
const posts = ref([])

onMounted(async () => {
  const response = await fetch('/posts.json')
  posts.value = await response.json()
})
</script>

<template>
  <div class="cv9im cpn01 cjx0x c7mbx cj439" data-aos-easing="ease-out-cubic" data-aos-duration="500"
       data-aos-delay="0">

    <!-- Page wrapper -->
    <div class="cp4zc c4i7i chg82 cmxqt">

      <!-- Site header -->
      <header class="cd7c9 ce83r crb4e c3yre">
        <div class="cwq08 cui38 cc4l3 cxnjg">
          <div class="c3as5 cpccj cewtd cmxqt cdiok">

            <!-- Site branding -->
            <div class="c3r53 cb6q3">
              <!-- Logo -->
              <a class="block ckuoi cgylk czxk3 cebnw" href="index.html" aria-label="Cruip">
                <svg class="c6urr cive7 cxllq" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg">
                  <path
                      d="M15.25 4.116c.039.899-.51.468-.79.629-.894.524-1.491 2.04-2.612 2.125-.423.87-1.121.898-1.874 1.503-.327.256-.463.839-.756 1.097l-3.694 3.27a2.395 2.395 0 0 1-.44.314c-.378.219-.656.717-1.096.81-.475.106-1.601-.775-2.633-2.012-.825-1.587-.025-1.924.518-2.525.916-1.022 2.48-2.064 3.585-2.753.843-.537 1.677-1.13 2.59-1.482.935-.357 1.779-.842 2.738-1.041.7-.141 1.522.063 2.206 0a9.596 9.596 0 0 1 2.258.065M30.676 3.646c-.06 1.046-1.038.955-1.593 1.363C27.32 6.31 25.8 8.656 23.63 9.583c-1.07 1.412-2.411 1.952-4.056 3.254-.711.56-1.21 1.417-1.877 1.965-2.887 2.381-5.668 4.524-8.64 6.823-.303.236-.646.468-1.008.697-.834.528-1.675 1.394-2.543 1.77-.95.413-2.376-.279-3.375-1.544-.43-1.849 1.112-2.657 2.38-3.737 2.13-1.82 5.33-4.012 7.558-5.536 1.707-1.17 3.395-2.426 5.138-3.43 1.789-1.03 3.439-2.179 5.224-3.063 1.303-.643 2.758-.96 4.038-1.53a40.762 40.762 0 0 1 4.207-1.606M30.386 14.346c.229.918-.566.8-.896 1.136-1.048 1.058-1.721 3.056-3.254 3.7-.563 1.17-1.522 1.532-2.603 2.507-.464.426-.731 1.128-1.177 1.542-1.94 1.77-3.91 3.263-6.082 4.772a6.36 6.36 0 0 1-.748.43c-.618.313-1.24.914-1.901 1.065-.731.161-1.856-.807-2.662-2.199-.401-1.784.715-2.129 1.6-2.818 1.49-1.15 3.693-2.49 5.192-3.486 1.154-.755 2.247-1.633 3.417-2.292 1.2-.68 2.244-1.52 3.44-2.128.868-.448 1.927-.61 2.79-1.029.92-.447 1.873-.85 2.884-1.2"></path>
                </svg>
              </a>
            </div>

            <!-- Desktop navigation -->
            <nav class="csvbf cm9ae cv4f1">

              <!-- Desktop menu links -->
              <ul class="co3jc cpccj cc7kb cmxqt cymr7">
                <li>
                  <a class="c8byp cjtfg ceywl cpn01 cpccj cgylk cy5nw czxk3 cebnw c9oso cmxqt cuy8x cpet4"
                     href="pricing.html">Pricing</a>
                </li>
                <li>
                  <a class="c8byp cjtfg ceywl cpn01 cpccj cgylk cy5nw czxk3 cebnw c9oso cmxqt cuy8x cpet4"
                     href="about.html">About</a>
                </li>
                <li>
                  <a class="c8byp cjtfg ceywl cpn01 cpccj cgylk cy5nw czxk3 cebnw c9oso cmxqt cuy8x cpet4"
                     href="blog.html">Blog</a>
                </li>
                <li>
                  <a class="c8byp cjtfg ceywl cpn01 cpccj cgylk cy5nw czxk3 cebnw c9oso cmxqt cuy8x cpet4"
                     href="wall-of-love.html">Wall of Love</a>
                </li>
                <!-- 1st level: hover -->
                <li class="ctd17" x-data="{ open: false }" @mouseenter="open = true" @mouseleave="open = false">
                  <a class="ceywl cpn01 cpccj cgylk cy5nw czxk3 cebnw c9oso cmxqt cuy8x cpet4" href="#0"
                     aria-haspopup="true" :aria-expanded="open" @focus="open = true" @focusout="open = false"
                     @click.prevent="" aria-expanded="false">
                    Resources
                    <svg class="cnygm c4sqn c20g7 c6urr c3r53 coc2c cy8g3 cg1yg" viewBox="0 0 12 12"
                         xmlns="http://www.w3.org/2000/svg">
                      <path
                          d="M10.28 4.305L5.989 8.598 1.695 4.305A1 1 0 00.28 5.72l5 5a1 1 0 001.414 0l5-5a1 1 0 10-1.414-1.414z"></path>
                    </svg>
                  </a>
                  <!-- 2nd level: hover -->
                  <ul class="cnf9a ciufj cd7c9 cciiv cj439 csdza ct7bo ccpoi ct7tf cpet4" x-show="open"
                      x-transition:enter="cebnw ch6f7 cc4ps cuxdo" x-transition:enter-start="cyixi c7pni"
                      x-transition:enter-end="c03gd cid49" x-transition:leave="cebnw ch6f7 cc4ps"
                      x-transition:leave-start="c03gd" x-transition:leave-end="cyixi" style="display: none;">
                    <li>
                      <a class="cjtfg ch02g confi cy5nw c35dk cmxqt cxnjg cpet4" href="404.html" @focus="open = true"
                         @focusout="open = false">404</a>
                    </li>
                    <li>
                      <a class="cjtfg ch02g confi cy5nw c35dk cmxqt cxnjg cpet4" href="support.html"
                         @focus="open = true" @focusout="open = false">Support</a>
                    </li>
                  </ul>
                </li>
              </ul>

              <!-- Desktop sign in links -->
              <ul class="cpccj cc6z4 cc7kb cmxqt cymr7">
                <li>
                  <a class="c8byp cjtfg ceywl cpn01 cpccj cgylk cy5nw czxk3 cebnw c9oso cmxqt cuy8x cpet4"
                     href="signin.html">Sign in</a>
                </li>
                <li>
                  <a class="c8q3m cmbhb ckuoi cpccj cgylk cy5nw czxk3 cebnw c9oso cuuxz cmxqt cuy8x cpet4"
                     href="request-demo.html">Request Demo <span
                      class="co5k7 cgu87 cs01c ckuoi cgylk czxk3 coc2c">-&gt;</span></a>
                </li>
              </ul>

            </nav>

            <!-- Mobile menu -->
            <div class="ca6e5 cmxqt" x-data="{ expanded: false }">

              <!-- Hamburger button -->
              <button class="cddv9" :class="{ 'active': expanded }" @click.stop="expanded = !expanded"
                      aria-controls="mobile-nav" :aria-expanded="expanded" aria-expanded="false">
                <span class="ctg7a">Menu</span>
                <svg class="cwtrp c9p59 c6urr cmo7l cssmu" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                  <rect y="4" width="24" height="2"></rect>
                  <rect y="11" width="24" height="2"></rect>
                  <rect y="18" width="24" height="2"></rect>
                </svg>
              </button>

              <!-- Mobile navigation -->
              <nav id="mobile-nav" class="cefnj cmyiy cd7c9 cciiv cdiod cj439 cgvj7 ce83r cei4k co8ir"
                   @click.away="expanded = false" @keydown.escape.window="expanded = false" x-show="expanded"
                   x-transition:enter="cebnw ch6f7 cc4ps cuxdo" x-transition:enter-start="cyixi c7pni"
                   x-transition:enter-end="c03gd cid49" x-transition:leave="cebnw ch6f7 cc4ps"
                   x-transition:leave-start="c03gd" x-transition:leave-end="cyixi" style="display: none;">
                <ul class="cxnjg cpet4">
                  <li>
                    <a class="cjtfg cpn01 cy5nw cmxqt cpet4" href="pricing.html">Pricing</a>
                  </li>
                  <li>
                    <a class="cjtfg cpn01 cy5nw cmxqt cpet4" href="about.html">About</a>
                  </li>
                  <li>
                    <a class="cjtfg cpn01 cy5nw cmxqt cpet4" href="blog.html">Blog</a>
                  </li>
                  <li>
                    <a class="cjtfg cpn01 cy5nw cmxqt cpet4" href="wall-of-love.html">Wall of Love</a>
                  </li>
                  <li class="c3elr cv2nt cfqxn c3bxe cpet4">
                    <span class="cjtfg cpn01 cy5nw cmxqt cpet4">Resources</span>
                    <ul class="cozz0">
                      <li>
                        <a class="cjtfg ch02g cy5nw c35dk cmxqt cpet4" href="404.html">404</a>
                      </li>
                      <li>
                        <a class="cjtfg ch02g cy5nw c35dk cmxqt cpet4" href="support.html">Support</a>
                      </li>
                    </ul>
                  </li>
                  <li>
                    <a class="cjtfg cpn01 cy5nw ce83r cmxqt cpet4" href="signin.html">Sign in</a>
                  </li>
                  <li>
                    <a class="ckuoi cy5nw cuuxz cmxqt cpet4" href="request-demo.html">Request Demo <span
                        class="co5k7 cgu87 cs01c ckuoi cgylk czxk3 coc2c">-&gt;</span></a>
                  </li>
                </ul>
              </nav>

            </div>

          </div>
        </div>
      </header>

      <!-- Page content -->
      <main class="cymr7">

        <!-- Hero -->
        <section class="ctd17">

          <!-- Dark background -->
          <div class="clupn cdw1p chtks cd7c9 c7hvf ct2qg" aria-hidden="true"></div>

          <div class="cwq08 ctd17 cui38 cc4l3 cucgo">
            <div class="c3h2d co43u cmy8r cvs2i">

              <!-- Hero content -->
              <div class="cl21a comxp c8n8h cuaiw cevdo c4nar cbr49 cz9ju csvbf cc4l3">

                <!-- Content -->
                <div class="c1bkb cdgxc csxy5 aos-init aos-animate" data-aos="fade-right">
                  <h1 class="c4ryg cy7k1 cc3ji c708p">Create stunning web experiences</h1>
                  <p class="c20g7 csj8k c47r3">Our landing page template works on all devices, so you only have to set
                    it up once, and get beautiful results forever.</p>
                  <div class="cq8r7 c5w3o c9074 c8fxx cpxiy c9qrd cy7gz cwm2b cc4l3">
                    <div>
                      <a class="cly6v cd857 cv4pf ce83r cuuxz cy3fp" href="request-demo.html">
                        Request Demo <span class="co5k7 cgu87 cs01c c6wde cgylk czxk3 coc2c">-&gt;</span>
                      </a>
                    </div>
                    <div>
                      <a class="ciksj cafxj cv4pf ce83r cy3fp" href="#0">Explore Product</a>
                    </div>
                  </div>
                </div>

                <!-- Hero image -->
                <div x-data="{ modalExpanded: false }" data-aos="fade-left" class="aos-init aos-animate">
                  <!-- Image -->
                  <div class="cni8m cpccj cmxqt">
                    <div class="ctd17">
                      <div class="cdw1p coa3w ceivd cmq04 cd7c9 c0hop c7hvf ct2qg cap31 c39ws" aria-hidden="true"></div>
                      <img class="comxp cc4l3" src="https://preview.cruip.com/tidy/images/hero-image-01.jpg" width="540"
                           height="405" alt="Hero">
                    </div>
                    <button class="cd7c9 cuuxz" @click.prevent="modalExpanded = true" aria-controls="modal">
                      <svg class="c6urr c5nmn cvas6 cuuxz cdiok cn59r" viewBox="0 0 88 88"
                           xmlns="http://www.w3.org/2000/svg">
                        <circle class="coxqe cgylk czxk3 cv4pf c7y72 cebnw" cx="44" cy="44" r="44"></circle>
                        <path class="ckuoi"
                              d="M52 44a.999.999 0 00-.427-.82l-10-7A1 1 0 0040 37V51a.999.999 0 001.573.82l10-7A.995.995 0 0052 44V44c0 .001 0 .001 0 0z"></path>
                      </svg>
                    </button>
                  </div>

                  <!-- Modal backdrop -->
                  <div class="cj32x cfruv ca1m2 c7hvf cw3ae caw21" x-show="modalExpanded"
                       x-transition:enter="cebnw ch6f7 cc4ps" x-transition:enter-start="cyixi"
                       x-transition:enter-end="c03gd" x-transition:leave="cebnw ch6f7 cp4l5"
                       x-transition:leave-start="c03gd" x-transition:leave-end="cyixi" aria-hidden="true"
                       style="display: none;"></div>

                  <!-- Modal dialog -->
                  <div id="modal" class="cp4zc cni8m cpccj cui38 c7hvf cw3ae caw21 cmxqt cucgo" role="dialog"
                       aria-modal="true" aria-labelledby="modal-headline" x-show="modalExpanded"
                       x-transition:enter="cebnw ch6f7 cc4ps" x-transition:enter-start="cyixi ctrey"
                       x-transition:enter-end="c03gd cy8ky" x-transition:leave="cebnw ch6f7 cc4ps"
                       x-transition:leave-start="c03gd cy8ky" x-transition:leave-end="cyixi ctrey"
                       style="display: none;">
                    <div class="cgbom cgc3h cwq08 cj439 ce83r" @click.away="modalExpanded = false"
                         @keydown.escape.window="modalExpanded = false">
                      <video x-init="$watch('modalExpanded', value => value ? $el.play() : $el.pause())"
                             class="c58z8 ce83r" width="1920" height="1080" loop="" controls="" __idm_id__="3997697">
                        <source src="https://preview.cruip.com/tidy/videos/video.mp4" type="video/mp4">
                        Your browser does not support the video tag.
                      </video>
                    </div>
                  </div>

                </div>
              </div>

            </div>
          </div>
        </section>

        <!-- Features blocks -->
        <section>
          <div class="cwq08 cui38 cc4l3 cucgo">
            <div class="c65y5 c4m2n">

              <!-- Items -->
              <div class="ctsjt cy425 cdby5 csp63 cs5xq caw9y ctd17 coqeb cc4l3 co4pk cv19t" data-aos-id-blocks="">

                <!-- Lines decoration -->
                <div class="cdw1p cp8e8 cd7c9 csvbf c7hvf cv4f1 cc8vg" aria-hidden="true">
                  <div class="catbc cctpv chemp cy4fy czlxh ctmo0 ce83r"></div>
                  <div class="catbc cctpv chemp cy4fy czlxh ctmo0 ce83r"></div>
                  <div class="catbc cctpv chemp cy4fy czlxh ctmo0 ce83r"></div>
                  <div class="catbc cctpv chemp cy4fy czlxh ctmo0 ce83r"></div>
                </div>

                <!-- 1st item -->
                <div class="ctd17 aos-init aos-animate" data-aos="fade-up" data-aos-anchor="[data-aos-id-blocks]">
                  <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" t="1729312002332" class="icon" viewBox="0 0 1024 1024" version="1.1" p-id="3597" width="200" height="200"><path d="M928 192v32H400l-64 64H32v-96a64 64 0 0 1 64-64h768a64 64 0 0 1 64 64z" fill="#1B45AF" p-id="3598"/><path d="M400 224l-64 64H32v544a64 64 0 0 0 64 64h768a64 64 0 0 0 64-64V224zM208 736a32 32 0 1 1 32-32 32 32 0 0 1-32 32z m160 0a32 32 0 1 1 32-32 32 32 0 0 1-32 32z m10.56-165.44A128 128 0 0 1 288 608h-128v-128h256a128 128 0 0 1-37.44 90.56zM800 816H576v-80h224z" fill="#CEE6F4" p-id="3599"/><path d="M992 224v608a64 64 0 0 1-64 64h-64a64 64 0 0 0 64-64V224z" fill="#ACD5EA" p-id="3600"/><path d="M992 192v32h-64v-32a64 64 0 0 0-64-64h64a64 64 0 0 1 64 64z" fill="#0A2872" p-id="3601"/><path d="M416 480a128 128 0 0 1-128 128h-128v-128z" fill="#1B45AF" p-id="3602"/><path d="M208 704m-32 0a32 32 0 1 0 64 0 32 32 0 1 0-64 0Z" fill="#0A2872" p-id="3603"/><path d="M368 704m-32 0a32 32 0 1 0 64 0 32 32 0 1 0-64 0Z" fill="#0A2872" p-id="3604"/><path d="M576 736h224v80H576z" fill="#458C28" p-id="3605"/><path d="M32 752a16 16 0 0 1-16-16V192a80 80 0 0 1 80-80h240a16 16 0 0 1 0 32H96a48 48 0 0 0-48 48v544a16 16 0 0 1-16 16z" fill="#0D182D" p-id="3606"/><path d="M864 912H96a80 80 0 0 1-80-80v-32a16 16 0 0 1 32 0v32a48 48 0 0 0 48 48h768a48 48 0 0 0 48-48V192a48 48 0 0 0-48-48H400a16 16 0 0 1 0-32h464a80 80 0 0 1 80 80v640a80 80 0 0 1-80 80z" fill="#0D182D" p-id="3607"/><path d="M928 912h-64a16 16 0 0 1 0-32 48 48 0 0 0 48-48V192a48 48 0 0 0-48-48 16 16 0 0 1 0-32h64a80 80 0 0 1 80 80v384a16 16 0 0 1-32 0V192a48 48 0 0 0-48-48 80 80 0 0 1 16 48v640a80 80 0 0 1-16 48 48 48 0 0 0 48-48V640a16 16 0 0 1 32 0v192a80 80 0 0 1-80 80z" fill="#0D182D" p-id="3608"/><path d="M336 304H48a16 16 0 0 1 0-32h281.44l59.2-59.36A16 16 0 0 1 400 208h592a16 16 0 0 1 0 32H406.56l-59.2 59.36A16 16 0 0 1 336 304z" fill="#0D182D" p-id="3609"/><path d="M128 224H112a16 16 0 0 1 0-32h16a16 16 0 0 1 0 32z" fill="#458C28" p-id="3610"/><path d="M208 224h-16a16 16 0 0 1 0-32h16a16 16 0 0 1 0 32z" fill="#D1B339" p-id="3611"/><path d="M288 224h-16a16 16 0 0 1 0-32h16a16 16 0 0 1 0 32z" fill="#D30B32" p-id="3612"/><path d="M288 624h-128a16 16 0 0 1-16-16v-128a16 16 0 0 1 16-16h64a16 16 0 0 1 0 32h-48v96h112a112 112 0 0 0 110.88-96H288a16 16 0 0 1 0-32h128a16 16 0 0 1 16 16 144 144 0 0 1-144 144z" fill="#0D182D" p-id="3613"/><path d="M368 688h-144a80 80 0 0 1-80-80v-144a32 32 0 0 0-32-32 16 16 0 0 1 0-32 64 64 0 0 1 64 64v144a48 48 0 0 0 48 48h144a16 16 0 0 1 0 32z" fill="#0D182D" p-id="3614"/><path d="M208 752a48 48 0 1 1 48-48 48 48 0 0 1-48 48z m0-64a16 16 0 1 0 16 16 16 16 0 0 0-16-16zM368 752a48 48 0 1 1 48-48 48 48 0 0 1-48 48z m0-64a16 16 0 1 0 16 16 16 16 0 0 0-16-16zM800 832H576a16 16 0 0 1-16-16v-80a16 16 0 0 1 16-16h224a16 16 0 0 1 16 16v80a16 16 0 0 1-16 16z m-208-32h192v-48H592zM832 400H544a16 16 0 0 1 0-32h288a16 16 0 0 1 0 32zM832 480H544a16 16 0 0 1 0-32h288a16 16 0 0 1 0 32zM832 560H544a16 16 0 0 1 0-32h288a16 16 0 0 1 0 32zM832 640H544a16 16 0 0 1 0-32h288a16 16 0 0 1 0 32z" fill="#0D182D" p-id="3615"/></svg>
                  <h3 class="c4ryg chiic cv4op">Lập trình Website</h3>
                  <p class="csmmp cg9j4">Tạo ra các trang web và ứng dụng web. Nó bao gồm việc sử dụng các ngôn ngữ lập
                    trình như HTML, CSS, JavaScript và các framework như Vue.js, React.js để xây dựng giao diện người
                    dùng và xử lý logic phía máy chủ. Mục tiêu là tạo ra các trang web tương tác, thân thiện với người
                    dùng và đáp ứng nhanh chóng.</p>
                </div>

                <!-- 2nd item -->
                <div class="ctd17 aos-init aos-animate" data-aos="fade-up" data-aos-anchor="[data-aos-id-blocks]"
                     data-aos-delay="100">
                  <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" t="1729311947045" class="icon" viewBox="0 0 1024 1024" version="1.1" p-id="6366" width="200" height="200"><path d="M816 96v832a64 64 0 0 1-51.2 64 66.72 66.72 0 0 1-12.8 0H208a64 64 0 0 1-64-64V96a64 64 0 0 1 64-64h544a64 64 0 0 1 64 64z" fill="#1B45AF" p-id="6367"/><path d="M880 96v832a64 64 0 0 1-64 64h-51.2a64 64 0 0 0 51.2-64V96a64 64 0 0 0-64-64h-19.2a66.72 66.72 0 0 0-12.8 0h96a64 64 0 0 1 64 64z" fill="#0A2872" p-id="6368"/><path d="M752 112v800a16 16 0 0 1-16 16H224a16 16 0 0 1-16-16V112a16 16 0 0 1 16-16h80l48 48h256l48-48h80a16 16 0 0 1 16 16z" fill="#CEE6F4" p-id="6369"/><path d="M752 928H208V768a544 544 0 0 0 544-544z" fill="#ACD5EA" p-id="6370"/><path d="M424 88.64m-24 0a24 24 0 1 0 48 0 24 24 0 1 0-48 0Z" fill="#798ACC" p-id="6371"/><path d="M536 88.64m-24 0a24 24 0 1 0 48 0 24 24 0 1 0-48 0Z" fill="#798ACC" p-id="6372"/><path d="M315.36 84.64A16 16 0 0 0 304 80h-80a32 32 0 0 0-32 32v800a32 32 0 0 0 32 32h512a32 32 0 0 0 32-32v-64a16 16 0 0 0-32 0v64H224V112h73.44l43.2 43.36A16 16 0 0 0 352 160h256a16 16 0 0 0 11.36-4.64L662.56 112H736v656a16 16 0 0 0 32 0V112a32 32 0 0 0-32-32h-80a16 16 0 0 0-11.36 4.64L601.44 128H358.56z" fill="#0D182D" p-id="6373"/><path d="M424 88m-24 0a24 24 0 1 0 48 0 24 24 0 1 0-48 0Z" fill="#76B4E2" p-id="6374"/><path d="M536 88m-24 0a24 24 0 1 0 48 0 24 24 0 1 0-48 0Z" fill="#76B4E2" p-id="6375"/><path d="M880 176a16 16 0 0 0 16-16V96a80 80 0 0 0-80-80H208a80 80 0 0 0-80 80v296a16 16 0 0 0 32 0V96a48 48 0 0 1 48-48h544a48 48 0 0 1 48 48v832a48 48 0 0 1-48 48H208a48 48 0 0 1-48-48V472a16 16 0 0 0-32 0V928a80 80 0 0 0 80 80h608a80 80 0 0 0 80-80V240a16 16 0 0 0-32 0v688a48 48 0 0 1-48 48 80 80 0 0 0 16-48V96a80 80 0 0 0-16-48 48 48 0 0 1 48 48v64a16 16 0 0 0 16 16z" fill="#0D182D" p-id="6376"/><path d="M272 256m32 0l32 0q32 0 32 32l0 32q0 32-32 32l-32 0q-32 0-32-32l0-32q0-32 32-32Z" fill="#B7041E" p-id="6377"/><path d="M592 256m32 0l32 0q32 0 32 32l0 32q0 32-32 32l-32 0q-32 0-32-32l0-32q0-32 32-32Z" fill="#D1B339" p-id="6378"/><path d="M432 256m32 0l32 0q32 0 32 32l0 32q0 32-32 32l-32 0q-32 0-32-32l0-32q0-32 32-32Z" fill="#1B45AF" p-id="6379"/><path d="M272 464m32 0l32 0q32 0 32 32l0 32q0 32-32 32l-32 0q-32 0-32-32l0-32q0-32 32-32Z" fill="#2C7013" p-id="6380"/><path d="M592 464m32 0l32 0q32 0 32 32l0 32q0 32-32 32l-32 0q-32 0-32-32l0-32q0-32 32-32Z" fill="#B7041E" p-id="6381"/><path d="M432 464m32 0l32 0q32 0 32 32l0 32q0 32-32 32l-32 0q-32 0-32-32l0-32q0-32 32-32Z" fill="#D1B339" p-id="6382"/><path d="M432 672m32 0l32 0q32 0 32 32l0 32q0 32-32 32l-32 0q-32 0-32-32l0-32q0-32 32-32Z" fill="#2C7013" p-id="6383"/><path d="M272 672m32 0l32 0q32 0 32 32l0 32q0 32-32 32l-32 0q-32 0-32-32l0-32q0-32 32-32Z" fill="#1B45AF" p-id="6384"/></svg>
                  <h3 class="c4ryg chiic cv4op">Lập trình Mobile</h3>
                  <p class="csmmp cg9j4">Quá trình phát triển các ứng dụng di động cho các thiết bị như điện thoại thông
                    minh và máy tính bảng. Nó bao gồm việc sử dụng các ngôn ngữ lập trình như Java, Swift, và Kotlin,
                    cùng với các framework như React Native và Flutter để xây dựng các ứng dụng di động đa nền tảng. Mục
                    tiêu là tạo ra các ứng dụng di động hiệu quả, thân thiện với người dùng và có hiệu suất cao.</p>
                </div>

                <!-- 3rd item -->
                <div class="ctd17 aos-init aos-animate" data-aos="fade-up" data-aos-anchor="[data-aos-id-blocks]"
                     data-aos-delay="200">
                  <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" t="1729312033213" class="icon" viewBox="0 0 1024 1024" version="1.1" p-id="3761" width="200" height="200"><path d="M896 464v368a64 64 0 0 1-64 64H96a64 64 0 0 1-64-64V320a64 64 0 0 1 64-64h672v272h64a64 64 0 0 0 64-64z" fill="#1B45AF" p-id="3762"/><path d="M32 400h864v128a64 64 0 0 1-64 64H96a64 64 0 0 1-64-64v-128z" fill="#0A2872" p-id="3763"/><path d="M944 256a48 48 0 0 0-48 48v160a64 64 0 0 1-64 64h-64V256zM768 256v272H96a64 64 0 0 1-64-64v-144a64 64 0 0 1 64-64z" fill="#1B45AF" p-id="3764"/><path d="M400 128a48 48 0 0 0-48 48v80h-64v-80a48 48 0 0 1 48-48zM640 176v80h-64v-80a48 48 0 0 0-48-48h64a48 48 0 0 1 48 48z" fill="#AA9335" p-id="3765"/><path d="M224 736a115.84 115.84 0 0 1-64-103.52V256h128v376.48A115.84 115.84 0 0 1 224 736z" fill="#D1B339" p-id="3766"/><path d="M224 592m-16 0a16 16 0 1 0 32 0 16 16 0 1 0-32 0Z" fill="#1B45AF" p-id="3767"/><path d="M224 656m-16 0a16 16 0 1 0 32 0 16 16 0 1 0-32 0Z" fill="#1B45AF" p-id="3768"/><path d="M768 256v376.48A115.84 115.84 0 0 1 704 736a115.84 115.84 0 0 1-64-103.52V256z" fill="#D1B339" p-id="3769"/><path d="M704 592m-16 0a16 16 0 1 0 32 0 16 16 0 1 0-32 0Z" fill="#1B45AF" p-id="3770"/><path d="M704 656m-16 0a16 16 0 1 0 32 0 16 16 0 1 0-32 0Z" fill="#1B45AF" p-id="3771"/><path d="M192 896H96a64 64 0 0 1-64-64v-96a160 160 0 0 1 160 160zM896 736v96a64 64 0 0 1-64 64h-96a160 160 0 0 1 160-160z" fill="#D1B339" p-id="3772"/><path d="M992 736v96a64 64 0 0 1-64 64h-96a64 64 0 0 0 64-64v-96z" fill="#AA9335" p-id="3773"/><path d="M992 304v432h-96V304a48 48 0 0 1 96 0z" fill="#0A2872" p-id="3774"/><path d="M160 448h128v80h-128zM640 448h128v80h-128z" fill="#AA9335" p-id="3775"/><path d="M224 592m-16 0a16 16 0 1 0 32 0 16 16 0 1 0-32 0Z" fill="#0D182D" p-id="3776"/><path d="M224 656m-16 0a16 16 0 1 0 32 0 16 16 0 1 0-32 0Z" fill="#0D182D" p-id="3777"/><path d="M704 592m-16 0a16 16 0 1 0 32 0 16 16 0 1 0-32 0Z" fill="#0D182D" p-id="3778"/><path d="M704 656m-16 0a16 16 0 1 0 32 0 16 16 0 1 0-32 0Z" fill="#0D182D" p-id="3779"/><path d="M989.28 258.72A64 64 0 0 0 944 240H656v-64a64 64 0 0 0-64-64H336a64 64 0 0 0-64 64v64H96a80 80 0 0 0-80 80v16a16 16 0 0 0 32 0v-16a48 48 0 0 1 48-48h48v240H96a48 48 0 0 1-48-48v-64a16 16 0 0 0-32 0v432a80 80 0 0 0 80 80h144a16 16 0 0 0 0-32h-32a176 176 0 0 0-160-159.2V528a78.72 78.72 0 0 0 48 16h48v88.48a130.72 130.72 0 0 0 72.8 117.76 16 16 0 0 0 14.4 0A130.72 130.72 0 0 0 304 632.48V544h176a16 16 0 0 0 0-32H304V272h320v32a16 16 0 0 0 32 0v-32h96v160h-96v-64a16 16 0 0 0-32 0v144h-80a16 16 0 0 0 0 32h80v88.48a131.04 131.04 0 0 0 72.8 117.76 16 16 0 0 0 14.4 0A131.04 131.04 0 0 0 784 632.48V544h48a90.24 90.24 0 0 0 14.88-1.44l4.48-1.12a92.8 92.8 0 0 0 9.44-3.04l4.8-2.08a83.36 83.36 0 0 0 8.32-4.48l4.16-2.56L880 528v192a176 176 0 0 0-160 160H304a16 16 0 0 0 0 32h624a80 80 0 0 0 80-80V304a64 64 0 0 0-18.72-45.28zM175.04 880H96a48 48 0 0 1-48-48v-79.04A144 144 0 0 1 175.04 880zM272 272v160h-96V272z m0 360.48a99.36 99.36 0 0 1-48 85.28 99.36 99.36 0 0 1-48-85.28V544h96zM176 512v-48h96v48z m128-336a32 32 0 0 1 32-32h8.64a65.76 65.76 0 0 0-3.36 6.72 61.76 61.76 0 0 0-3.2 10.56 16 16 0 0 0 0 2.72A68.48 68.48 0 0 0 336 176v64h-32z m64 0a32 32 0 0 1 32-32h128a32 32 0 0 1 32 32v64H368z m224 0a68.48 68.48 0 0 0-1.12-11.52 16 16 0 0 0 0-2.72 61.76 61.76 0 0 0-3.2-10.56 65.76 65.76 0 0 0-4.32-7.2H592a32 32 0 0 1 32 32v64h-32z m384 128v416h-64V304a32 32 0 0 1 32-32 32 32 0 0 1 32 32zM656 464h96v48h-96z m48 253.76a99.36 99.36 0 0 1-48-85.28V544h96v88.48a99.36 99.36 0 0 1-48 85.28zM784 512V272h104.64a65.76 65.76 0 0 0-3.36 6.72 61.76 61.76 0 0 0-3.2 10.56 16 16 0 0 0 0 2.72A68.48 68.48 0 0 0 880 304v160a48 48 0 0 1-48 48z m96 240.96V832a48 48 0 0 1-48 48h-79.04A144 144 0 0 1 880 752.96zM928 880h-32l1.28-1.92 2.56-4.16a83.36 83.36 0 0 0 4.48-8.32c0-1.6 1.44-3.2 2.08-4.8a92.8 92.8 0 0 0 3.04-9.44c0-1.6 0-3.04 1.12-4.48A90.24 90.24 0 0 0 912 832v-80h64v80a48 48 0 0 1-48 48z" fill="#0D182D" p-id="3780"/></svg>
                  <h3 class="c4ryg chiic cv4op">Lập trình Tool</h3>
                  <p class="csmmp cg9j4">Quá trình phát triển các công cụ phần mềm để hỗ trợ các nhiệm vụ cụ thể trong
                    công việc hoặc cuộc sống hàng ngày. Nó bao gồm việc sử dụng các ngôn ngữ lập trình như Python,
                    JavaScript, và C# để tạo ra các ứng dụng giúp tự động hóa các quy trình, phân tích dữ liệu, hoặc
                    quản lý hệ thống. Mục tiêu là tạo ra các công cụ hiệu quả, dễ sử dụng và có thể tùy chỉnh theo nhu
                    cầu của người dùng.</p>
                </div>

                <!-- 4th item -->
                <div class="ctd17 aos-init aos-animate" data-aos="fade-up" data-aos-anchor="[data-aos-id-blocks]"
                     data-aos-delay="300">
                  <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" t="1729312211186" class="icon" viewBox="0 0 1024 1024" version="1.1" p-id="4269" width="200" height="200"><path d="M816 336h-133.92l17.28 19.84A203.04 203.04 0 0 1 728.96 400 211.2 211.2 0 0 1 752 496H304a211.2 211.2 0 0 1 23.04-96 203.04 203.04 0 0 1 29.6-44.16L374.08 336H240a64 64 0 0 0-64 64v448h176l16 16h144l16-16h352V400a64 64 0 0 0-64-64z m0 435.2a16 16 0 0 1-16 12.8H256a16 16 0 0 1-16-12.8 40 40 0 0 1 40-35.2 38.88 38.88 0 0 1 25.92 9.6A56 56 0 0 1 360 704a53.44 53.44 0 0 1 24.8 5.92A80 80 0 0 1 464 640a75.36 75.36 0 0 1 16 1.6V560h96v81.6a75.36 75.36 0 0 1 16-1.6 80 80 0 0 1 80 69.92 53.44 53.44 0 0 1 24-5.92 56 56 0 0 1 54.08 41.6 38.88 38.88 0 0 1 25.92-9.6 40 40 0 0 1 40 34.88z" fill="#76B4E2" p-id="4270"/><path d="M816 416v352a16 16 0 0 1 0 2.88A40 40 0 0 0 776 736a38.88 38.88 0 0 0-25.92 9.6A56 56 0 0 0 696 704a53.44 53.44 0 0 0-24.8 5.92A80 80 0 0 0 592 640a75.36 75.36 0 0 0-16 1.6V560h-96v81.6a75.36 75.36 0 0 0-16-1.6 80 80 0 0 0-79.2 69.92A53.44 53.44 0 0 0 360 704a56 56 0 0 0-54.08 41.6 38.88 38.88 0 0 0-25.92-9.6 40 40 0 0 0-40 35.04 17.76 17.76 0 0 1 0-3.04V416a16 16 0 0 1 16-16h71.04A211.2 211.2 0 0 0 304 496h448a211.2 211.2 0 0 0-23.04-96H800a16 16 0 0 1 16 16z" fill="#CEE6F4" p-id="4271"/><path d="M944 848v48a48 48 0 0 1-48 48h-48a64 64 0 0 1-64-64 32 32 0 0 1 32-32z" fill="#1B45AF" p-id="4272"/><path d="M944 400v448h-64V400a64 64 0 0 0-64-64h64a64 64 0 0 1 64 64z" fill="#5EA2CC" p-id="4273"/><path d="M848 944H144a64 64 0 0 1-64-64 32 32 0 0 1 32-32h240l16 16h144l16-16h288a32 32 0 0 0-32 32 64 64 0 0 0 64 64z" fill="#1B45AF" p-id="4274"/><path d="M816 770.88a16 16 0 0 1-16 12.8H256a16 16 0 0 1-16-12.8A40 40 0 0 1 280 736a38.88 38.88 0 0 1 25.92 9.6A56 56 0 0 1 360 704a53.44 53.44 0 0 1 24.8 5.92A80 80 0 0 1 464 640a75.36 75.36 0 0 1 16 1.6V560h96v81.6a75.36 75.36 0 0 1 16-1.6 80 80 0 0 1 80 69.92 53.44 53.44 0 0 1 24-5.92 56 56 0 0 1 54.08 41.6 38.88 38.88 0 0 1 25.92-9.6 40 40 0 0 1 40 34.88z" fill="#D1B339" p-id="4275"/><path d="M659.84 768l26.24-13.76a21.6 21.6 0 0 1 9.92-2.24 24 24 0 0 1 22.56 16z m-248 0l4.8-38.24A48 48 0 0 1 464 688a50.88 50.88 0 0 1 9.12 0L512 745.28V608a16 16 0 0 1 16-16 16 16 0 0 1 16 16v137.28l38.88-56.48A50.88 50.88 0 0 1 592 688a48 48 0 0 1 48 41.76l4.8 38.24z m-74.4 0a24 24 0 0 1 22.56-16 21.6 21.6 0 0 1 9.92 2.24l26.24 13.76z" fill="#AA9335" p-id="4276"/><path d="M640 249.92V464a32 32 0 0 1-32 32H448a32 32 0 0 1-32-32V249.92A185.44 185.44 0 0 1 528 80a186.24 186.24 0 0 1 32 17.28A183.36 183.36 0 0 1 606.4 144l3.04 4.32A184.64 184.64 0 0 1 640 249.92z" fill="#ACD5EA" p-id="4277"/><path d="M592 201.92V416a32 32 0 0 1-32 32h-144V249.92A185.44 185.44 0 0 1 528 80a186.24 186.24 0 0 1 32 17.28l2.08 2.88A184.64 184.64 0 0 1 592 201.92z" fill="#CEE6F4" p-id="4278"/><path d="M752 496h-144a32 32 0 0 0 32-32V288l42.08 48 17.28 19.84A203.04 203.04 0 0 1 728.96 400 211.2 211.2 0 0 1 752 496z" fill="#D30B32" p-id="4279"/><path d="M448 496h-144a211.2 211.2 0 0 1 23.04-96 203.04 203.04 0 0 1 29.6-44.16l11.36-12.96 6.08-6.88L416 288v176a32 32 0 0 0 32 32zM704 496h-96a32 32 0 0 0 32-32v-121.28l11.36 13.12A203.04 203.04 0 0 1 680.96 400 211.2 211.2 0 0 1 704 496z" fill="#B7041E" p-id="4280"/><path d="M400 496h-96a211.2 211.2 0 0 1 23.04-96 203.04 203.04 0 0 1 29.6-44.16l11.36-12.96V464a32 32 0 0 0 32 32z" fill="#D30B32" p-id="4281"/><path d="M606.4 144a110.56 110.56 0 0 1-78.4 32 98.56 98.56 0 0 1-24-2.72A108.8 108.8 0 0 1 449.6 144a181.44 181.44 0 0 1 54.4-51.36A170.72 170.72 0 0 1 528 80a183.04 183.04 0 0 1 78.4 64z" fill="#B7041E" p-id="4282"/><path d="M504.64 173.12A108.8 108.8 0 0 1 449.6 144a181.44 181.44 0 0 1 54.4-51.36 163.04 163.04 0 0 1 14.88 10.24 39.84 39.84 0 0 1-14.24 70.24z" fill="#D30B32" p-id="4283"/><path d="M608 496l-16 64h-128l-16-64h160zM384.8 709.92A53.6 53.6 0 0 0 384 720M672 720a53.6 53.6 0 0 0 0-10.08" fill="#CEE6F4" p-id="4284"/><path d="M576 352a48 48 0 0 1-93.92 13.92A49.6 49.6 0 0 1 480 352a48 48 0 0 1 48-48 49.6 49.6 0 0 1 13.92 2.08A48 48 0 0 1 576 352z" fill="#5EA2CC" p-id="4285"/><path d="M544 320a48 48 0 0 1-48 48 49.6 49.6 0 0 1-13.92-2.08A49.6 49.6 0 0 1 480 352a48 48 0 0 1 48-48 49.6 49.6 0 0 1 13.92 2.08A49.6 49.6 0 0 1 544 320z" fill="#76B4E2" p-id="4286"/><path d="M896 960h-48a80 80 0 0 1-80-80 48 48 0 0 1 48-48h128a16 16 0 0 1 16 16v48a64 64 0 0 1-64 64z m-80-96a14.88 14.88 0 0 0-11.04 4.64A16 16 0 0 0 800 880a48 48 0 0 0 48 48h48a32 32 0 0 0 32-32v-32z" fill="#0D182D" p-id="4287"/><path d="M944 864h-64a16 16 0 0 1-16-16V672a16 16 0 0 1 32 0v160h32V400a48 48 0 0 0-48-48 80 80 0 0 1 16 48v208a16 16 0 0 1-32 0V400a48 48 0 0 0-48-48 16 16 0 0 1 0-32h64a80 80 0 0 1 80 80v448a16 16 0 0 1-16 16zM848 960H144a80 80 0 0 1-80-80 48 48 0 0 1 48-48h240a16 16 0 0 1 11.36 4.64l11.2 11.36h130.88l11.2-11.36A16 16 0 0 1 528 832h96a16 16 0 0 1 0 32h-89.44l-11.2 11.36A16 16 0 0 1 512 880h-144a16 16 0 0 1-11.36-4.64l-11.2-11.36H112a14.88 14.88 0 0 0-11.04 4.64A16 16 0 0 0 96 880a48 48 0 0 0 48 48h640a80 80 0 0 1-16-48 48 48 0 0 1 2.72-16H688a16 16 0 0 1 0-32h128a16 16 0 0 1 0 32 14.88 14.88 0 0 0-11.04 4.64A16 16 0 0 0 800 880a48 48 0 0 0 48 48 16 16 0 0 1 0 32z" fill="#0D182D" p-id="4288"/><path d="M816 786.72a16 16 0 0 1-16-13.76A24.16 24.16 0 0 0 776 752a23.04 23.04 0 0 0-16 5.6 16 16 0 0 1-26.08-7.84A39.84 39.84 0 0 0 696 720a37.44 37.44 0 0 0-17.44 4.16 16 16 0 0 1-22.56-12.32A64 64 0 0 0 592 656a61.44 61.44 0 0 0-12.64 1.28 16 16 0 0 1-19.36-16V576h-64v65.6a16 16 0 0 1-19.36 16 67.04 67.04 0 0 0-38.24 4 16 16 0 1 1-12.8-29.12A92.48 92.48 0 0 1 464 624v-64a16 16 0 0 1 16-16h96a16 16 0 0 1 16 16v64a96 96 0 0 1 90.88 65.28 71.36 71.36 0 0 1 74.88 33.76 57.12 57.12 0 0 1 42.08 2.4V416h-46.4a227.04 227.04 0 0 1 14.56 80 16 16 0 0 1-16 16H304a16 16 0 0 1-16-16 227.04 227.04 0 0 1 14.56-80H256v96a16 16 0 0 1-32 0v-96a32 32 0 0 1 32-32h71.04a16 16 0 0 1 14.24 23.36A194.56 194.56 0 0 0 320 480h416a194.56 194.56 0 0 0-20.64-72.64 16 16 0 0 1 13.6-23.36H800a32 32 0 0 1 32 32v352a24.16 24.16 0 0 1 0 5.12 16 16 0 0 1-16 13.6zM240 787.04a16 16 0 0 1-16-13.44 30.4 30.4 0 0 1 0-5.6V576a16 16 0 0 1 32 0v149.44a57.44 57.44 0 0 1 42.24-2.4A72.16 72.16 0 0 1 360 688a73.28 73.28 0 0 1 13.28 1.28 91.2 91.2 0 0 1 14.24-27.04 16 16 0 0 1 22.56-2.88 16 16 0 0 1 2.88 22.4 64 64 0 0 0-12.96 30.08 16 16 0 0 1-8.48 12.32 16 16 0 0 1-14.72 0A37.44 37.44 0 0 0 360 720a39.84 39.84 0 0 0-38.56 29.76 16 16 0 0 1-10.88 11.2 16 16 0 0 1-15.2-3.36 23.04 23.04 0 0 0-16-5.6A23.84 23.84 0 0 0 256 772.96a16 16 0 0 1-16 14.08z" fill="#0D182D" p-id="4289"/><path d="M800 800H256a32 32 0 0 1-32-25.76 17.76 17.76 0 0 1 0-3.04 9.12 9.12 0 0 1 0-2.08A55.84 55.84 0 0 1 280 720a53.92 53.92 0 0 1 18.24 3.04A72.16 72.16 0 0 1 360 688a73.28 73.28 0 0 1 13.28 1.28 91.2 91.2 0 0 1 14.24-27.04 16 16 0 0 1 22.56-2.88 16 16 0 0 1 2.88 22.4 64 64 0 0 0-12.96 30.08 16 16 0 0 1-8.48 12.32 16 16 0 0 1-14.72 0A37.44 37.44 0 0 0 360 720a39.84 39.84 0 0 0-38.56 29.76 16 16 0 0 1-10.88 11.2 16 16 0 0 1-15.2-3.36 23.04 23.04 0 0 0-16-5.6 24.16 24.16 0 0 0-22.72 16h542.08a24.16 24.16 0 0 0-22.72-16 23.04 23.04 0 0 0-16 5.6 16 16 0 0 1-26.08-7.84A39.84 39.84 0 0 0 696 720a37.44 37.44 0 0 0-17.44 4.16 16 16 0 0 1-22.56-12.32A64 64 0 0 0 592 656a61.44 61.44 0 0 0-12.64 1.28 16 16 0 0 1-19.36-16V576h-64v65.6a16 16 0 0 1-19.36 16 67.04 67.04 0 0 0-38.24 4 16 16 0 1 1-12.8-29.12A92.48 92.48 0 0 1 464 624v-64a16 16 0 0 1 16-16h96a16 16 0 0 1 16 16v64a96 96 0 0 1 90.88 65.28 71.36 71.36 0 0 1 74.88 33.76A53.92 53.92 0 0 1 776 720a56 56 0 0 1 55.52 48 9.12 9.12 0 0 1 0 2.08 21.76 21.76 0 0 1 0 3.36A32 32 0 0 1 800 800z" fill="#0D182D" p-id="4290"/><path d="M512 880h-144a16 16 0 0 1-11.36-4.64l-11.2-11.36H176a16 16 0 0 1-16-16V400a80 80 0 0 1 80-80h134.08a16 16 0 0 1 12 26.56L368 366.4a182.24 182.24 0 0 0-27.2 40.64A195.04 195.04 0 0 0 320 480h416a194.56 194.56 0 0 0-20.64-72.64A183.04 183.04 0 0 0 688 366.4l-17.28-19.84a16 16 0 0 1 11.36-26.56H816a80 80 0 0 1 80 80v208a16 16 0 0 1-32 0V400a48 48 0 0 0-48-48h-98.88a231.84 231.84 0 0 1 26.24 40.96A228.96 228.96 0 0 1 768 496a16 16 0 0 1-16 16H304a16 16 0 0 1-16-16 229.28 229.28 0 0 1 24.8-103.36A222.08 222.08 0 0 1 338.88 352H240a48 48 0 0 0-48 48v432h160a16 16 0 0 1 11.36 4.64l11.2 11.36h130.88l11.2-11.36A16 16 0 0 1 528 832h96a16 16 0 0 1 0 32h-89.44l-11.2 11.36A16 16 0 0 1 512 880z m368-16H688a16 16 0 0 1 0-32h176V672a16 16 0 0 1 32 0v176a16 16 0 0 1-16 16z m-80-64H256a32 32 0 0 1-32-25.76 17.76 17.76 0 0 1 0-3.04 9.12 9.12 0 0 1 0-2.08A55.84 55.84 0 0 1 280 720a53.92 53.92 0 0 1 18.24 3.04A72.16 72.16 0 0 1 360 688a73.28 73.28 0 0 1 13.28 1.28 91.2 91.2 0 0 1 14.24-27.04 16 16 0 0 1 22.56-2.88 16 16 0 0 1 2.88 22.4 64 64 0 0 0-12.96 30.08 16 16 0 0 1-8.48 12.32 16 16 0 0 1-14.72 0A37.44 37.44 0 0 0 360 720a39.84 39.84 0 0 0-38.56 29.76 16 16 0 0 1-10.88 11.2 16 16 0 0 1-15.2-3.36 23.04 23.04 0 0 0-16-5.6 24.16 24.16 0 0 0-22.72 16h542.08a24.16 24.16 0 0 0-22.72-16 23.04 23.04 0 0 0-16 5.6 16 16 0 0 1-26.08-7.84A39.84 39.84 0 0 0 696 720a37.44 37.44 0 0 0-17.44 4.16 16 16 0 0 1-22.56-12.32A64 64 0 0 0 592 656a61.44 61.44 0 0 0-12.64 1.28 16 16 0 0 1-19.36-16V576h-64v65.6a16 16 0 0 1-19.36 16 67.04 67.04 0 0 0-38.24 4 16 16 0 1 1-12.8-29.12A92.48 92.48 0 0 1 464 624v-64a16 16 0 0 1 16-16h96a16 16 0 0 1 16 16v64a96 96 0 0 1 90.88 65.28 71.36 71.36 0 0 1 74.88 33.76A53.92 53.92 0 0 1 776 720a56 56 0 0 1 55.52 48 9.12 9.12 0 0 1 0 2.08 21.76 21.76 0 0 1 0 3.36A32 32 0 0 1 800 800z" fill="#0D182D" p-id="4291"/><path d="M608 512H448a48 48 0 0 1-48-48V256a16 16 0 0 1 32 0v208a16 16 0 0 0 16 16h160a16 16 0 0 0 16-16V249.92a167.36 167.36 0 0 0-28-92.96c0-1.12-1.44-2.24-2.24-3.36A166.88 166.88 0 0 0 528 97.6a165.92 165.92 0 0 0-65.28 55.36 168 168 0 0 0-26.4 58.72 16 16 0 1 1-31.04-7.36 201.12 201.12 0 0 1 116.48-139.04 16 16 0 0 1 12.48 0 197.76 197.76 0 0 1 85.28 69.44 45.44 45.44 0 0 1 3.2 4.64A200.16 200.16 0 0 1 656 249.92V464a48 48 0 0 1-48 48z" fill="#0D182D" p-id="4292"/><path d="M752 512h-144a16 16 0 0 1 0-32 16 16 0 0 0 16-16V288a16 16 0 0 1 28-10.56l59.36 67.84a224 224 0 0 1 32 48A228.96 228.96 0 0 1 768 496a16 16 0 0 1-16 16z m-98.72-32H736a194.56 194.56 0 0 0-20.64-72.64A183.04 183.04 0 0 0 688 366.4l-32-35.84V464a48 48 0 0 1-2.72 16zM448 512h-144a16 16 0 0 1-16-16 229.28 229.28 0 0 1 24.8-103.36 224 224 0 0 1 32-48l59.36-67.84A16 16 0 0 1 432 288v176a16 16 0 0 0 16 16 16 16 0 0 1 0 32z m-128-32h82.08a48 48 0 0 1-2.08-16v-133.28l-32 35.68a182.24 182.24 0 0 0-27.2 40.64A195.04 195.04 0 0 0 320 480zM528 192a126.4 126.4 0 0 1-89.6-36.8 16 16 0 0 1-1.92-20.48 197.76 197.76 0 0 1 85.28-69.44 16 16 0 0 1 12.48 0 197.76 197.76 0 0 1 85.28 69.44 16 16 0 0 1-1.92 20.48A126.4 126.4 0 0 1 528 192z m-56.64-50.4a98.72 98.72 0 0 0 113.28 0A167.36 167.36 0 0 0 528 97.6a167.36 167.36 0 0 0-56.64 44z" fill="#0D182D" p-id="4293"/><path d="M592 576h-128a16 16 0 0 1-16-12.16l-16-64a16 16 0 0 1 2.88-13.76A16 16 0 0 1 448 480h160a16 16 0 0 1 12.64 6.08 16 16 0 0 1 2.88 13.76l-16 64A16 16 0 0 1 592 576z m-115.52-32h103.04l8-32h-119.04zM480 736a16 16 0 0 1-16-16v-78.4a16 16 0 1 1 32 0V720a16 16 0 0 1-16 16zM576 736a16 16 0 0 1-16-16v-78.4a16 16 0 1 1 32 0V720a16 16 0 0 1-16 16zM384 736a16 16 0 0 1-16-16 69.92 69.92 0 0 1 1.12-13.12 16 16 0 0 1 32 6.08A34.72 34.72 0 0 0 400 720a16 16 0 0 1-16 16zM672 736a16 16 0 0 1-16-16 34.72 34.72 0 0 0 0-7.04 16 16 0 1 1 32-6.08 69.92 69.92 0 0 1 0 13.12 16 16 0 0 1-16 16zM528 416a64 64 0 0 1-64-64 16 16 0 0 1 32 0 32 32 0 1 0 32-32 29.92 29.92 0 0 0-10.24 1.76 16 16 0 0 1-11.52-29.76A57.76 57.76 0 0 1 528 288a64 64 0 0 1 0 128z" fill="#0D182D" p-id="4294"/></svg>
                  <h3 class="c4ryg chiic cv4op">SEO Web</h3>
                  <p class="csmmp cg9j4">SEO (Search Engine Optimization) là quá trình tối ưu hóa trang web để cải thiện
                    thứ hạng của nó trên các công cụ tìm kiếm như Google. Nó bao gồm việc sử dụng các kỹ thuật như tối
                    ưu hóa từ khóa, xây dựng liên kết, và cải thiện tốc độ tải trang để tăng cường khả năng hiển thị và
                    thu hút lưu lượng truy cập tự nhiên. Mục tiêu là đạt được thứ hạng cao hơn trong kết quả tìm kiếm và
                    thu hút nhiều khách hàng tiềm năng hơn.</p>
                </div>

                <!-- 5th item -->
                <div class="ctd17 aos-init aos-animate" data-aos="fade-up" data-aos-anchor="[data-aos-id-blocks]"
                     data-aos-delay="400">
                  <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" t="1729312171923" class="icon" viewBox="0 0 1024 1024" version="1.1" p-id="4105" width="200" height="200"><path d="M704 688H320a16 16 0 0 1-14.24-8.64 16 16 0 0 1 1.12-16l192-272a16 16 0 0 1 26.24 0l192 272a16 16 0 0 1 1.12 16A16 16 0 0 1 704 688z m-353.12-32h322.24L512 427.68z" fill="#5EA2CC" p-id="4106"/><path d="M667.84 292.32a16 16 0 0 1-6.08-1.28A18.4 18.4 0 0 1 656 288a16 16 0 0 1-4.64-11.36 16.8 16.8 0 0 1 4.64-11.36 16 16 0 0 1 17.44-3.36 18.4 18.4 0 0 1 5.28 3.36 16.8 16.8 0 0 1 4.64 11.36 16 16 0 0 1-1.28 6.08 18.4 18.4 0 0 1-3.36 5.28 16 16 0 0 1-10.88 4.32zM848 570.08a16 16 0 0 1 14.88-16.96 16 16 0 0 1 17.12 14.88 16 16 0 0 1-16 17.12 16 16 0 0 1-16-15.04zM838.4 512a16 16 0 0 1 11.84-19.2 16 16 0 0 1 19.36 11.68 16 16 0 0 1-11.84 19.36 14.56 14.56 0 0 1-3.68 0 16 16 0 0 1-15.68-11.84z m-18.72-55.52a16 16 0 0 1 8.16-21.12 16 16 0 0 1 21.12 8.16 16 16 0 0 1-8.16 21.12 16 16 0 0 1-6.4 1.44 16 16 0 0 1-14.72-9.28z m-28.16-51.36a16 16 0 0 1 4.32-21.12 16 16 0 0 1 22.24 4.48 16 16 0 0 1-4.48 22.24 16 16 0 0 1-8.8 2.56 16 16 0 0 1-13.28-7.84z m-36.64-45.76a16 16 0 0 1 0-22.72 16 16 0 0 1 22.56 0 16 16 0 0 1 0 22.72 16 16 0 0 1-11.04 4.32 16 16 0 0 1-11.52-4z m-44.16-38.56a16 16 0 0 1-3.52-22.4 16 16 0 0 1 22.4-3.36 16 16 0 0 1 3.36 22.4 16 16 0 0 1-12.96 6.4 16 16 0 0 1-9.28-2.72zM861.92 646.72a16 16 0 0 1-11.36-4.64 16 16 0 0 1-4.64-11.36 16.8 16.8 0 0 1 4.64-11.36 16 16 0 0 1 5.28-3.36 16 16 0 0 1 9.28-0.96l2.88 0.96a12.16 12.16 0 0 1 2.88 1.44 25.28 25.28 0 0 1 2.4 1.92 16 16 0 0 1 3.36 5.28 16 16 0 0 1 1.28 6.08 13.44 13.44 0 0 1-1.28 6.08 14.4 14.4 0 0 1-8.64 8.64 16 16 0 0 1-6.08 1.28zM162.08 646.72a16 16 0 0 1-6.08-1.28 14.4 14.4 0 0 1-8.64-8.64 16 16 0 0 1-1.28-6.08 16.8 16.8 0 0 1 4.64-11.36 18.4 18.4 0 0 1 5.28-3.36 14.72 14.72 0 0 1 12.16 0 18.4 18.4 0 0 1 5.28 3.36 16.8 16.8 0 0 1 4.64 11.36 16 16 0 0 1-1.12 6.08 23.36 23.36 0 0 1-3.52 5.28 18.4 18.4 0 0 1-5.28 3.36 16 16 0 0 1-6.08 1.28zM160 585.28a16 16 0 0 1-14.88-16.96 16 16 0 0 1 16.96-14.88 16 16 0 0 1 13.92 16.96 16 16 0 0 1-16 14.88z m6.4-61.12a16 16 0 0 1-11.68-19.2 16 16 0 0 1 19.36-11.84 16 16 0 0 1 11.36 18.88 16 16 0 0 1-16 12.16 16 16 0 0 1-3.36 0z m17.12-59.04a16 16 0 0 1-8.32-20.96 16 16 0 0 1 21.12-8.32 16 16 0 0 1 8.32 21.12 16 16 0 0 1-14.72 9.6 16 16 0 0 1-6.72-1.44z m27.04-55.04a16 16 0 0 1-4.48-22.24 16 16 0 0 1 21.92-3.84 16 16 0 0 1 4.48 22.24 16 16 0 0 1-13.44 7.2 16 16 0 0 1-8.8-3.36z m36.16-49.6a16 16 0 0 1 0-22.72 16 16 0 0 1 22.72 0 16 16 0 0 1 0 22.72 16 16 0 0 1-11.68 4.8 16 16 0 0 1-11.36-4.8z m44.32-42.56a16 16 0 0 1 3.36-22.4 16 16 0 0 1 22.4 3.36 16 16 0 0 1-3.36 22.4 16 16 0 0 1-9.6 3.04 16 16 0 0 1-13.12-6.4zM356.16 292.32a16 16 0 0 1-16-16 16 16 0 1 1 32 0 16 16 0 0 1-1.12 6.08A23.36 23.36 0 0 1 368 288a16 16 0 0 1-11.84 4.32zM326.56 907.36a16 16 0 0 1-6.08-1.28 18.4 18.4 0 0 1-5.28-3.36 16 16 0 0 1-3.36-17.44 18.4 18.4 0 0 1 3.36-5.28 16 16 0 0 1 5.28-3.36 16 16 0 0 1 17.44 3.36 18.4 18.4 0 0 1 3.36 5.28 13.44 13.44 0 0 1 1.28 6.08 16 16 0 0 1-16 16zM496 944a16 16 0 0 1 16-16 16 16 0 0 1 16 16 16 16 0 0 1-16 16 16 16 0 0 1-16-16z m64.96-3.04a16 16 0 0 1 12.96-18.56 16 16 0 0 1 18.56 12.8 16 16 0 0 1-12.8 18.72H576a16 16 0 0 1-15.2-12.96z m-116.48 12.8a16 16 0 0 1-12.8-18.56 16 16 0 0 1 18.56-12.8 16 16 0 0 1 12.8 18.56 16 16 0 0 1-16 13.12zM624 926.24a16 16 0 0 1 9.12-20.8 16 16 0 0 1 20.8 9.28 16 16 0 0 1-9.12 20.64 14.72 14.72 0 0 1-5.76 1.12 16 16 0 0 1-15.04-10.24z m-245.28 8.96a16 16 0 0 1-9.12-20.64 16 16 0 0 1 20.64-9.12 16 16 0 0 1 9.76 20.64 16 16 0 0 1-14.88 10.24 14.72 14.72 0 0 1-6.24-1.12zM697.44 907.36a16 16 0 0 1-6.08-1.28 18.4 18.4 0 0 1-5.28-3.36 16 16 0 0 1-3.36-17.44 18.4 18.4 0 0 1 3.36-5.28 16 16 0 0 1 22.72 0 18.4 18.4 0 0 1 3.36 5.28 16 16 0 0 1-3.36 17.44 18.4 18.4 0 0 1-5.28 3.36 16 16 0 0 1-6.08 1.28z" fill="#D1B339" p-id="4107"/><path d="M368 784a160 160 0 1 1-68.64-131.36A160 160 0 0 1 368 784zM976 784a160 160 0 1 1-68.64-131.36A160 160 0 0 1 976 784zM672 240a160 160 0 0 1-268.64 117.28 163.2 163.2 0 0 1-22.88-26.24A160 160 0 1 1 672 240z" fill="#AA9335" p-id="4108"/><path d="M328 744a160 160 0 0 1-251.36 131.36 160 160 0 0 1 222.72-222.72 160 160 0 0 1 28.64 91.36zM936 744a160 160 0 0 1-251.36 131.36 160 160 0 0 1 222.72-222.72 160 160 0 0 1 28.64 91.36zM632 200a160 160 0 0 1-251.52 131.04 160 160 0 0 1 222.88-222.4 160 160 0 0 1 28.64 91.36z" fill="#D1B339" p-id="4109"/><path d="M576 208a64 64 0 0 1-122.24 26.24A62.88 62.88 0 0 1 448 208a64 64 0 0 1 64-64 62.88 62.88 0 0 1 26.24 5.76A64 64 0 0 1 576 208z" fill="#ACD5EA" p-id="4110"/><path d="M620.64 357.28a160 160 0 0 1-217.28 0 112 112 0 0 1 217.28 0z" fill="#76B4E2" p-id="4111"/><path d="M880 752a64 64 0 0 1-122.24 26.24A62.88 62.88 0 0 1 752 752a64 64 0 0 1 64-64 62.88 62.88 0 0 1 26.24 5.76A64 64 0 0 1 880 752z" fill="#ACD5EA" p-id="4112"/><path d="M924.64 901.28a160 160 0 0 1-217.28 0 112 112 0 0 1 217.28 0z" fill="#76B4E2" p-id="4113"/><path d="M272 752a64 64 0 0 1-122.24 26.24A62.88 62.88 0 0 1 144 752a64 64 0 0 1 64-64 62.88 62.88 0 0 1 26.24 5.76A64 64 0 0 1 272 752z" fill="#ACD5EA" p-id="4114"/><path d="M544 176a64 64 0 0 1-64 64 62.88 62.88 0 0 1-26.24-5.76A62.88 62.88 0 0 1 448 208a64 64 0 0 1 64-64 62.88 62.88 0 0 1 26.24 5.76A62.88 62.88 0 0 1 544 176zM848 720a64 64 0 0 1-64 64 62.88 62.88 0 0 1-26.24-5.76A62.88 62.88 0 0 1 752 752a64 64 0 0 1 64-64 62.88 62.88 0 0 1 26.24 5.76A62.88 62.88 0 0 1 848 720zM240 720a64 64 0 0 1-64 64 62.88 62.88 0 0 1-26.24-5.76A62.88 62.88 0 0 1 144 752a64 64 0 0 1 64-64 62.88 62.88 0 0 1 26.24 5.76A62.88 62.88 0 0 1 240 720z" fill="#CEE6F4" p-id="4115"/><path d="M316.64 901.28a160 160 0 0 1-217.28 0 112 112 0 0 1 217.28 0z" fill="#76B4E2" p-id="4116"/><path d="M208 960a176 176 0 1 1 176-176 176 176 0 0 1-176 176z m0-320a144 144 0 1 0 144 144 144 144 0 0 0-144-144zM816 960a176 176 0 1 1 176-176 176 176 0 0 1-176 176z m0-320a144 144 0 1 0 144 144 144 144 0 0 0-144-144zM512 416a176 176 0 0 1-176-176 177.6 177.6 0 0 1 3.52-35.68 16 16 0 0 1 32 6.4A147.68 147.68 0 0 0 368 240a144 144 0 1 0 26.88-83.52A16 16 0 1 1 368 137.92a176 176 0 1 1 263.52 231.2A174.72 174.72 0 0 1 512 416z" fill="#0D182D" p-id="4117"/><path d="M512 288a80 80 0 1 1 80-80 80 80 0 0 1-80 80z m0-128a48 48 0 1 0 48 48 48 48 0 0 0-48-48z" fill="#0D182D" p-id="4118"/><path d="M512 416a174.08 174.08 0 0 1-119.52-47.04 16 16 0 0 1-4.64-16 128 128 0 0 1 248.32 0 16 16 0 0 1-4.64 16A174.08 174.08 0 0 1 512 416z m-90.4-64a144 144 0 0 0 180.8 0 96 96 0 0 0-180.8 0zM816 832a80 80 0 1 1 80-80 80 80 0 0 1-80 80z m0-128a48 48 0 1 0 48 48 48 48 0 0 0-48-48z" fill="#0D182D" p-id="4119"/><path d="M816 960a174.08 174.08 0 0 1-119.52-47.04 16 16 0 0 1-4.64-16 128 128 0 0 1 26.72-52.16 16 16 0 1 1 24.32 20.8 94.88 94.88 0 0 0-17.28 30.4 144 144 0 0 0 180.8 0A96 96 0 0 0 816 832a101.28 101.28 0 0 0-29.12 4.48 16 16 0 1 1-9.6-30.4A129.44 129.44 0 0 1 816 800a128 128 0 0 1 124.16 97.44 16 16 0 0 1-4.64 16A174.08 174.08 0 0 1 816 960zM208 832a80 80 0 1 1 77.44-99.84 16 16 0 1 1-31.04 8 48 48 0 1 0-11.04 43.84 16 16 0 0 1 23.68 21.44A80 80 0 0 1 208 832z" fill="#0D182D" p-id="4120"/><path d="M208 960a174.08 174.08 0 0 1-119.52-47.04 16 16 0 0 1-4.64-16 128 128 0 0 1 248.32 0 16 16 0 0 1-4.64 16A174.08 174.08 0 0 1 208 960z m-90.4-64a144 144 0 0 0 180.8 0 96 96 0 0 0-180.8 0z" fill="#0D182D" p-id="4121"/></svg>
                  <h3 class="c4ryg chiic cv4op">Chạy quảng cáo</h3>
                  <p class="csmmp cg9j4">Chạy quảng cáo là quá trình tạo và quản lý các chiến dịch quảng cáo trên các
                    nền tảng trực tuyến như Google Ads, Facebook Ads, và Instagram Ads. Nó bao gồm việc thiết kế nội
                    dung quảng cáo, lựa chọn đối tượng mục tiêu, và tối ưu hóa chiến dịch để đạt được hiệu quả cao nhất.
                    Mục tiêu là tăng cường nhận diện thương hiệu và thu hút khách hàng tiềm năng.</p>
                </div>

                <!-- 6th item -->
                <div class="ctd17 aos-init aos-animate" data-aos="fade-up" data-aos-anchor="[data-aos-id-blocks]"
                     data-aos-delay="500">
                  <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" t="1729312237663" class="icon" viewBox="0 0 1024 1024" version="1.1" p-id="4440" width="200" height="200"><path d="M944 160v48H784v-48a80 80 0 1 1 160 0zM688 942.4v1.6H160a80 80 0 0 1-80-80v-48h544v48a80 80 0 0 0 64 78.4z" fill="#76B4E2" p-id="4441"/><path d="M784 688v176a80 80 0 0 1-80 80 75.36 75.36 0 0 1-16-1.6 80 80 0 0 1-64-78.4v-48H240v-64a541.12 541.12 0 0 0 320-104V736l48-48zM784 208v240h-55.68A541.28 541.28 0 0 0 784 208z" fill="#ACD5EA" p-id="4442"/><path d="M864 80a80 80 0 0 0-80 80v48a541.28 541.28 0 0 1-55.68 240H624a64 64 0 0 0-64 64v136A541.12 541.12 0 0 1 240 752V448h176l48 48V272a64 64 0 0 0-64-64H240v-48a80 80 0 0 1 80-80z" fill="#CEE6F4" p-id="4443"/><path d="M464 272v224l-48-48H144a64 64 0 0 1-64-64v-112a64 64 0 0 1 64-64h256a64 64 0 0 1 64 64zM944 512v112a64 64 0 0 1-64 64H608l-48 48V512a64 64 0 0 1 64-64h256a64 64 0 0 1 64 64z" fill="#AA9335" p-id="4444"/><path d="M464 272v176l-48-48H144a64 64 0 0 1-64-64v-64a64 64 0 0 1 64-64h256a64 64 0 0 1 64 64zM944 512v64a64 64 0 0 1-64 64H608l-48 48V512a64 64 0 0 1 64-64h256a64 64 0 0 1 64 64z" fill="#D1B339" p-id="4445"/><path d="M944 224H784a16 16 0 0 1-16-16v-48a96 96 0 1 1 192 0v48a16 16 0 0 1-16 16z m-144-32h128v-32a64 64 0 0 0-64-64 64 64 0 0 0-64 64zM688 960H160a96 96 0 0 1-96-96v-48a16 16 0 0 1 16-16h544a16 16 0 0 1 16 16v48a64 64 0 0 0 18.72 45.44 64 64 0 0 0 32 17.28 16 16 0 0 1 12.8 16V944a16 16 0 0 1-15.52 16zM96 832v32a64 64 0 0 0 64 64h472.32A96 96 0 0 1 608 864v-32zM240 704a16 16 0 0 1-16-16V448a16 16 0 0 1 16-16h176a16 16 0 0 1 11.36 4.64l20.64 20.8V272a48 48 0 0 0-48-48H240a16 16 0 0 1-16-16v-48a96 96 0 0 1 96-96h80a16 16 0 0 1 0 32h-80a64 64 0 0 0-64 64v32h144a80 80 0 0 1 80 80v224a16 16 0 0 1-9.92 14.72 16 16 0 0 1-17.44-3.36L409.44 464H256v224a16 16 0 0 1-16 16z" fill="#0D182D" p-id="4446"/><path d="M704 960a92.32 92.32 0 0 1-19.36-1.92A96 96 0 0 1 608 864v-32H240a16 16 0 0 1-16-16v-64a16 16 0 0 1 32 0v48h368a16 16 0 0 1 16 16v48a64 64 0 0 0 18.72 45.44A64 64 0 0 0 768 864V704h-32a16 16 0 0 1 0-32h48a16 16 0 0 1 16 16v176a96 96 0 0 1-96 96z" fill="#0D182D" p-id="4447"/><path d="M560 752a13.44 13.44 0 0 1-6.08-1.28A16 16 0 0 1 544 736V512a80 80 0 0 1 80-80h144V160a96 96 0 0 1 24.48-64H464a16 16 0 0 1 0-32h400a16 16 0 0 1 0 32 64 64 0 0 0-64 64v288a16 16 0 0 1-16 16H624a48 48 0 0 0-48 48v185.44l20.64-20.8A16 16 0 0 1 608 672h64a16 16 0 0 1 0 32h-57.44l-43.2 43.36A16 16 0 0 1 560 752z" fill="#0D182D" p-id="4448"/><path d="M464 512a16 16 0 0 1-11.36-4.64L409.44 464H144a80 80 0 0 1-80-80v-32a16 16 0 0 1 32 0v32a48 48 0 0 0 48 48h272a16 16 0 0 1 11.36 4.64l20.64 20.8V272a48 48 0 0 0-48-48H144a48 48 0 0 0-48 48v16a16 16 0 0 1-32 0v-16a80 80 0 0 1 80-80h256a80 80 0 0 1 80 80v224a16 16 0 0 1-9.92 14.72 13.44 13.44 0 0 1-6.08 1.28zM560 752a13.44 13.44 0 0 1-6.08-1.28A16 16 0 0 1 544 736V512a80 80 0 0 1 80-80h256a80 80 0 0 1 80 80v112a80 80 0 0 1-80 80h-144a16 16 0 0 1 0-32h144a48 48 0 0 0 48-48v-112a48 48 0 0 0-48-48H624a48 48 0 0 0-48 48v185.44l20.64-20.8A16 16 0 0 1 608 672h64a16 16 0 0 1 0 32h-57.44l-43.2 43.36A16 16 0 0 1 560 752z" fill="#0D182D" p-id="4449"/><path d="M168 328m-24 0a24 24 0 1 0 48 0 24 24 0 1 0-48 0Z" fill="#0D182D" p-id="4450"/><path d="M264 328m-24 0a24 24 0 1 0 48 0 24 24 0 1 0-48 0Z" fill="#0D182D" p-id="4451"/><path d="M360 328m-24 0a24 24 0 1 0 48 0 24 24 0 1 0-48 0Z" fill="#0D182D" p-id="4452"/><path d="M664 568m-24 0a24 24 0 1 0 48 0 24 24 0 1 0-48 0Z" fill="#0D182D" p-id="4453"/><path d="M760 568m-24 0a24 24 0 1 0 48 0 24 24 0 1 0-48 0Z" fill="#0D182D" p-id="4454"/><path d="M856 568m-24 0a24 24 0 1 0 48 0 24 24 0 1 0-48 0Z" fill="#0D182D" p-id="4455"/><path d="M704 224H544a16 16 0 0 1 0-32h160a16 16 0 0 1 0 32zM704 304H544a16 16 0 0 1 0-32h160a16 16 0 0 1 0 32zM704 384H544a16 16 0 0 1 0-32h160a16 16 0 0 1 0 32zM480 592H320a16 16 0 0 1 0-32h160a16 16 0 0 1 0 32zM480 672H320a16 16 0 0 1 0-32h160a16 16 0 0 1 0 32zM480 752H320a16 16 0 0 1 0-32h160a16 16 0 0 1 0 32z" fill="#0D182D" p-id="4456"/></svg>
                  <h3 class="c4ryg chiic cv4op">Viết bài</h3>
                  <p class="csmmp cg9j4">Tạo ra nội dung văn bản cho các mục đích khác nhau như blog, báo chí, hoặc tài
                    liệu kỹ thuật. Nó bao gồm việc nghiên cứu, lập kế hoạch, viết và chỉnh sửa để đảm bảo nội dung rõ
                    ràng, hấp dẫn và chính xác. Mục tiêu là truyền đạt thông tin một cách hiệu quả và thu hút sự quan
                    tâm của người đọc.</p>
                </div>
              </div>

            </div>
          </div>
        </section>

        <!-- Features 01 -->
        <section class="ctd17">

          <div class="cdw1p caqoh cgyl1 cd7c9 c7hvf c1fsr" aria-hidden="true"></div>

          <div class="cwq08 ctd17 cui38 cc4l3 cucgo">
            <div class="c65y5 c4m2n">

              <!-- Section header -->
              <div class="csxy5 cquxk cc4l3 cz6lp">
                <h2 class="c4ryg cpn01 cc3ji cgxhh">Built exclusively for you</h2>
                <p class="csmmp csj8k">Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia
                  deserunt mollit anim id est laborum — semper quis lectus nulla at volutpat diam ut venenatis.</p>
              </div>

              <!-- Section content -->
              <div class="cquxk cc4l3" x-data="{ tab: '1' }">

                <!-- Tabs buttons -->
                <div class="csiii c8ihi c28oh cz6lp cv19t">
                  <button class="cj32x csxy5" :class="tab === '1' || 'cdsks cbxqe'" @click="tab = '1'">
                    <div class="c4kmg c4psy c5dyz cj439 ci9ig">
                      <svg width="56" height="56" xmlns="http://www.w3.org/2000/svg">
                        <path fill="#2174EA" d="M20 20h6v16h-6z"></path>
                        <path fill-opacity=".64" fill="#5091EE" d="M29 20h3v16h-3zM35 20h1v16h-1z"></path>
                      </svg>
                    </div>
                    <div class="cpn01 ck3uh confi ca4ye">Internal Feedback</div>
                  </button>
                  <button class="cj32x csxy5 cdsks cbxqe" :class="tab === '2' || 'cdsks cbxqe'" @click="tab = '2'">
                    <div class="c4kmg c4psy c5dyz cj439 ci9ig">
                      <svg width="56" height="56" xmlns="http://www.w3.org/2000/svg">
                        <path fill-opacity=".64" fill="#5091EE" d="M33 23v8h3V20H25v3z"></path>
                        <path fill="#2174EA" d="M20 25h11v11H20z"></path>
                      </svg>
                    </div>
                    <div class="cpn01 ck3uh confi ca4ye">Internal Feedback</div>
                  </button>
                  <button class="cj32x csxy5 cdsks cbxqe" :class="tab === '3' || 'cdsks cbxqe'" @click="tab = '3'">
                    <div class="c4kmg c4psy c5dyz cj439 ci9ig">
                      <svg width="56" height="56" xmlns="http://www.w3.org/2000/svg">
                        <path fill-opacity=".64" fill="#5091EE" d="M20 27l7-7h-7z"></path>
                        <path fill="#2174EA" d="M29 20l7 7v-7z"></path>
                        <path fill-opacity=".64" fill="#5091EE" d="M36 29l-7 7h7z"></path>
                        <path fill="#2174EA" d="M27 36l-7-7v7z"></path>
                      </svg>
                    </div>
                    <div class="cpn01 ck3uh confi ca4ye">Internal Feedback</div>
                  </button>
                  <button class="cj32x csxy5 cdsks cbxqe" :class="tab === '4' || 'cdsks cbxqe'" @click="tab = '4'">
                    <div class="c4kmg c4psy c5dyz cj439 ci9ig">
                      <svg width="56" height="56" xmlns="http://www.w3.org/2000/svg">
                        <path d="M24 28h-4v4.9c0 1 .7 1.9 1.7 2.1 1.2.2 2.3-.8 2.3-2v-5z" fill-opacity=".64"
                              fill="#5091EE"></path>
                        <path d="M35 21h-8c-.6 0-1 .4-1 1v11c0 .7-.2 1.4-.6 2H33c1.7 0 3-1.3 3-3V22c0-.6-.4-1-1-1z"
                              fill="#2174EA"></path>
                      </svg>
                    </div>
                    <div class="cpn01 ck3uh confi ca4ye">Internal Feedback</div>
                  </button>
                </div>

                <!-- Tab items -->
                <div class="ctd17 chg82 cmxqt aos-init aos-animate" data-aos="fade-up">
                  <div x-show="tab === '1'" x-transition:enter="cebnw czxk3 c5adh c9yxr"
                       x-transition:enter-start="cyixi cbhm3" x-transition:enter-end="c03gd cid49"
                       x-transition:leave="cebnw czxk3 cjg84 cd7c9" x-transition:leave-start="c03gd cid49"
                       x-transition:leave-end="cyixi cz709">
                    <img class="cup1z cc4l3" src="https://preview.cruip.com/tidy/images/features-home-01.jpg"
                         width="768" height="474" alt="Features home 01">
                  </div>
                  <div x-show="tab === '2'" x-transition:enter="cebnw czxk3 c5adh c9yxr"
                       x-transition:enter-start="cyixi cbhm3" x-transition:enter-end="c03gd cid49"
                       x-transition:leave="cebnw czxk3 cjg84 cd7c9" x-transition:leave-start="c03gd cid49"
                       x-transition:leave-end="cyixi cz709" style="display: none;">
                    <img class="cup1z cc4l3" src="https://preview.cruip.com/tidy/images/features-home-01.jpg"
                         width="768" height="474" alt="Features home 02">
                  </div>
                  <div x-show="tab === '3'" x-transition:enter="cebnw czxk3 c5adh c9yxr"
                       x-transition:enter-start="cyixi cbhm3" x-transition:enter-end="c03gd cid49"
                       x-transition:leave="cebnw czxk3 cjg84 cd7c9" x-transition:leave-start="c03gd cid49"
                       x-transition:leave-end="cyixi cz709" style="display: none;">
                    <img class="cup1z cc4l3" src="https://preview.cruip.com/tidy/images/features-home-01.jpg"
                         width="768" height="474" alt="Features home 03">
                  </div>
                  <div x-show="tab === '4'" x-transition:enter="cebnw czxk3 c5adh c9yxr"
                       x-transition:enter-start="cyixi cbhm3" x-transition:enter-end="c03gd cid49"
                       x-transition:leave="cebnw czxk3 cjg84 cd7c9" x-transition:leave-start="c03gd cid49"
                       x-transition:leave-end="cyixi cz709" style="display: none;">
                    <img class="cup1z cc4l3" src="https://preview.cruip.com/tidy/images/features-home-01.jpg"
                         width="768" height="474" alt="Features home 04">
                  </div>
                </div>

              </div>

            </div>
          </div>
        </section>

        <!-- Features 02 -->
        <section>
          <div class="cwq08 cui38 cc4l3 cucgo">
            <div class="c3elr c65y5 cv2nt c4m2n">

              <!-- Section header -->
              <div class="csxy5 cquxk c54e1 cc4l3 cz6lp">
                <h2 class="c4ryg cpn01 cgxhh">The quick brown fox jumped over the lazy dog</h2>
              </div>

              <!-- Section content -->
              <div class="xl:space-x-18 ck0zt ci8h0 comxp c8n8h cevdo c4nar co8zu c04nu cz9ju chg82 cc4l3 cmxqt"
                   x-data="{ tab: '1' }">

                <!-- Tabs items (images) -->
                <div class="c218p cri0v cz9zg c3ira cijuu aos-init aos-animate" data-aos="fade-down">
                  <div class="ctd17 chg82 cmxqt">
                    <!-- Item 1 -->
                    <div class="ce83r" x-show="tab === '1'" x-transition:enter="cebnw czxk3 c5adh cuxdo c9yxr"
                         x-transition:enter-start="cyixi cbhm3" x-transition:enter-end="c03gd cid49"
                         x-transition:leave="cebnw czxk3 cjg84 cuxdo cd7c9" x-transition:leave-start="c03gd cid49"
                         x-transition:leave-end="cyixi cz709">
                      <img class="comxp cc4l3 ct7bo" src="https://preview.cruip.com/tidy/images/features-home-02.png"
                           width="540" height="620" alt="Features home 2 01">
                    </div>
                    <!-- Item 2 -->
                    <div class="ce83r" x-show="tab === '2'" x-transition:enter="cebnw czxk3 c5adh cuxdo c9yxr"
                         x-transition:enter-start="cyixi cbhm3" x-transition:enter-end="c03gd cid49"
                         x-transition:leave="cebnw czxk3 cjg84 cuxdo cd7c9" x-transition:leave-start="c03gd cid49"
                         x-transition:leave-end="cyixi cz709" style="display: none;">
                      <img class="comxp cc4l3 ct7bo" src="https://preview.cruip.com/tidy/images/features-home-02.png"
                           width="540" height="620" alt="Features home 2 02">
                    </div>
                    <!-- Item 3 -->
                    <div class="ce83r" x-show="tab === '3'" x-transition:enter="cebnw czxk3 c5adh cuxdo c9yxr"
                         x-transition:enter-start="cyixi cbhm3" x-transition:enter-end="c03gd cid49"
                         x-transition:leave="cebnw czxk3 cjg84 cuxdo cd7c9" x-transition:leave-start="c03gd cid49"
                         x-transition:leave-end="cyixi cz709" style="display: none;">
                      <img class="comxp cc4l3 ct7bo" src="https://preview.cruip.com/tidy/images/features-home-02.png"
                           width="540" height="620" alt="Features home 2 03">
                    </div>
                  </div>
                </div>

                <!-- Content -->
                <div class="cvbuf cz9zg aos-init aos-animate" data-aos="fade-up">
                  <div class="cdgxc csxy5 c47r3">
                    <h3 class="c4ryg cpn01 ci9ig cq8sc">Built exclusively for you</h3>
                    <p class="csmmp csj8k">Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia
                      deserunt mollit anim id est laborum — semper quis lectus nulla at volutpat diam ut venenatis.</p>
                  </div>
                  <!-- Tabs buttons -->
                  <div class="c5ud2 c47r3">
                    <button :class="tab !== '1' ? 'c5t34 cdsks cbxqe' : 'c0hop cxxj7 c03gd'"
                            class="cjg84 caw9y czxk3 cebnw cd9v1 c5dyz c0hop cj439 ct7bo ci9ig cmxqt cxnjg cowqg cxxj7 c03gd"
                            @click="tab = '1'">
                      <svg class="ckuoi c6urr c3r53 cb6q3 cpb3u cmvs9 cua0z" viewBox="0 0 16 16"
                           xmlns="http://www.w3.org/2000/svg">
                        <path d="M9.4 6.6c.8.8.8 2 0 2.8-.8.8-2 .8-2.8 0-.8-.8-5-7.8-5-7.8s7 4.2 7.8 5Z"></path>
                        <path
                            d="M8 16c-4.4 0-8-3.6-8-8 0-.6.4-1 1-1s1 .4 1 1c0 3.3 2.7 6 6 6s6-2.7 6-6-2.7-6-6-6c-.6 0-1-.4-1-1s.4-1 1-1c4.4 0 8 3.6 8 8s-3.6 8-8 8Z"></path>
                      </svg>
                      <div>
                        <div class="cpn01 cy5nw cp0cj">Internal Feedback</div>
                        <div class="csmmp">Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore
                          eu fugiat nulla pariatur velit.
                        </div>
                      </div>
                    </button>
                    <button :class="tab !== '2' ? 'c5t34 cdsks cbxqe' : 'c0hop cxxj7 c03gd'"
                            class="cjg84 caw9y czxk3 cebnw cd9v1 c5dyz c0hop cj439 ct7bo ci9ig cmxqt cxnjg cowqg c5t34 cdsks cbxqe"
                            @click="tab = '2'">
                      <svg class="ckuoi c6urr c3r53 cb6q3 cpb3u cmvs9 cua0z" viewBox="0 0 16 16"
                           xmlns="http://www.w3.org/2000/svg">
                        <path
                            d="M4.019 15.276.034 1.329A1.058 1.058 0 0 1 1.33.034L15.276 4.02c.896.299.996 1.494.1 1.893L8.8 8.8l-2.79 6.574c-.498.897-1.693.797-1.992-.1ZM2.525 2.525l2.69 9.463 1.892-4.383c.1-.199.299-.398.498-.498l4.383-1.893-9.463-2.69Z"></path>
                      </svg>
                      <div>
                        <div class="cpn01 cy5nw cp0cj">Internal Feedback</div>
                        <div class="csmmp">Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore
                          eu fugiat nulla pariatur velit.
                        </div>
                      </div>
                    </button>
                    <button :class="tab !== '3' ? 'c5t34 cdsks cbxqe' : 'c0hop cxxj7 c03gd'"
                            class="cjg84 caw9y czxk3 cebnw cd9v1 c5dyz c0hop cj439 ct7bo cmxqt cxnjg cowqg c5t34 cdsks cbxqe"
                            @click="tab = '3'">
                      <svg class="ckuoi c6urr c3r53 cb6q3 cpb3u cmvs9 cua0z" viewBox="0 0 16 16"
                           xmlns="http://www.w3.org/2000/svg">
                        <path
                            d="M15.686 5.71 10.291.3c-.4-.4-.999-.4-1.399 0a.97.97 0 0 0 0 1.403l.6.6L2.698 6.01l-1-1.002c-.4-.4-.999-.4-1.398 0a.97.97 0 0 0 0 1.403l1.498 1.502 2.398 2.404L.6 14.023 2 15.425l3.696-3.706 3.997 4.007c.5.5 1.199.2 1.398 0a.97.97 0 0 0 0-1.402l-.999-1.002 3.697-6.711.6.6c.599.602 1.199.201 1.398 0 .3-.4.3-1.1-.1-1.502Zm-7.193 6.11L4.196 7.511l6.695-3.706 1.298 1.302-3.696 6.711Z"></path>
                      </svg>
                      <div>
                        <div class="cpn01 cy5nw cp0cj">Internal Feedback</div>
                        <div class="csmmp">Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore
                          eu fugiat nulla pariatur velit.
                        </div>
                      </div>
                    </button>
                  </div>
                </div>

              </div>

            </div>
          </div>
        </section>

        <!-- Features 03 -->
        <section class="ctd17">

          <!-- Dark background -->
          <div class="clupn cdw1p chtks c7wsr cst1q cd7c9 c7hvf ct2qg c2p75" aria-hidden="true"></div>

          <div class="cwq08 ctd17 cui38 cc4l3 cucgo">
            <div class="c65y5 c4m2n">

              <!-- Section header -->
              <div class="csxy5 cquxk c54e1 cc4l3 cz6lp">
                <h2 class="c4ryg cy7k1 cgxhh">Simplify operating and manage with transparency</h2>
              </div>

              <!-- Section content -->
              <div class="cljwv comxp cqcp3 c4as4 caw9y coqeb cc4l3 cguqk cv19t">

                <!-- 1st article -->
                <article data-aos="fade-up" class="aos-init aos-animate">
                  <a class="block ctd17 cuuxz cc3ji cx2ha" href="#0">
                    <div class="chwia cv5ho cdw1p ck8gg cvk7y ceivd cjg84 c4ug2 cebnw cd7c9 c0hop ch6f7 c7hvf ct2qg"
                         aria-hidden="true"></div>
                    <div class="cp4zc">
                      <img class="clgwa csqag ckemv c5adh cebnw ch6f7 ce83r"
                           src="https://preview.cruip.com/tidy/images/features-home-3-01.jpg" width="342" height="342"
                           alt="News 01">
                    </div>
                    <div class="cugo1 cwbd8 c4kmg c8u3l cd7c9 cvrk6 cdx1x cdiok cn59r">
                      <svg class="c6urr cdiok cn59r" viewBox="0 0 64 64" xmlns="http://www.w3.org/2000/svg">
                        <path class="cv4pf"
                              d="m30.152 39.848.672-.408C32.24 33.632 33.92 32 35.96 26.768a10.714 10.714 0 0 0-.432-2.28c-.288-.096-.888-.336-1.44-.336-1.776.48-3.48 1.632-5.208 2.088-1.272.336-.576 2.352.36 3.312.672-.384 1.872-1.008 2.28-.96-1.248 2.112-3 6.12-3 7.704 0 .528-.48.816-.48 1.104 0 .288.12.6.144.936.384-.24.48-.12.48.264.264.192.672.504 1.032.816.144-.744.384-1.56.888-1.464l-.6 1.704c.072.072.12.144.168.192Z"></path>
                      </svg>
                    </div>
                  </a>
                  <h3 class="c4ryg chiic cv4op">
                    <a class="cic5i cbepq cpn01" href="#0">Advanced Features</a>
                  </h3>
                  <p class="csmmp cg9j4">Lorem ipsum is placeholder text used in the graphic, print, and publishing for
                    previewing layouts.</p>
                </article>

                <!-- 2nd article -->
                <article data-aos="fade-up" data-aos-delay="100" class="aos-init aos-animate">
                  <a class="block ctd17 cuuxz cc3ji cx2ha" href="#0">
                    <div class="chwia cv5ho cdw1p ck8gg cvk7y ceivd cjg84 c4ug2 cebnw cd7c9 c0hop ch6f7 c7hvf ct2qg"
                         aria-hidden="true"></div>
                    <div class="cp4zc">
                      <img class="clgwa csqag ckemv c5adh cebnw ch6f7 ce83r"
                           src="https://preview.cruip.com/tidy/images/features-home-3-02.jpg" width="342" height="342"
                           alt="News 02">
                    </div>
                    <div class="cugo1 cwbd8 c4kmg c8u3l cd7c9 cvrk6 cdx1x cdiok cn59r">
                      <svg class="c6urr cdiok cn59r" viewBox="0 0 64 64" xmlns="http://www.w3.org/2000/svg">
                        <path class="cv4pf"
                              d="M25.508 39.044c.312 0 .672-.024 1.008-.048-.096-.432.384-.528.816-.096 1.488-.216 3.12-.624 4.416-.888l.6-.624c1.104 0 .456.624 1.44.432.168-1.008.552-.456 1.92-1.176l.072.168c-.264.192-.72.408-1.152.576v.216c1.584-.528 1.848-1.32 2.928-1.464 1.224-.168 2.184-.048 2.52-.792l-1.728-.096-.168-.24h1.008l-.096-.216c-1.032 0-1.44-.168-2.4-.576-2.016.192-5.328.912-7.632.768 1.296-1.512 3.72-2.592 5.712-3.648.024.36-.384.6-.744.816l.072.216 1.344-.744c.048-.72.552-1.344 1.272-1.44.6-.744.864-1.776.864-2.76 0-1.08-1.2-2.208-3.024-2.208l.096-.264c-1.968.192-5.4.36-6.792 1.176-.504.288-.456.696-.792.984.48.36.024.528.504 1.2.624.888.648 1.488 1.152 1.2 1.056-.576 2.4-1.176 3.384-1.176.48 0 .864.168 1.104.504 0 1.488-6.744 3.792-9.288 7.632.48.096.312.48.072.84.504.768.84 1.728 1.512 1.728Zm7.344-5.976.912-.48-.048-.264-.912.6.048.144Zm7.08 3.216-.096-.216-1.128.216c.144.168.72.048 1.224 0Z"></path>
                      </svg>
                    </div>
                  </a>
                  <h3 class="c4ryg chiic cv4op">
                    <a class="cic5i cbepq cpn01" href="#0">Advanced Features</a>
                  </h3>
                  <p class="csmmp cg9j4">Lorem ipsum is placeholder text used in the graphic, print, and publishing for
                    previewing layouts.</p>
                </article>

                <!-- 3rd article -->
                <article data-aos="fade-up" data-aos-delay="200" class="aos-init aos-animate">
                  <a class="block ctd17 cuuxz cc3ji cx2ha" href="#0">
                    <div class="chwia cv5ho cdw1p ck8gg cvk7y ceivd cjg84 c4ug2 cebnw cd7c9 c0hop ch6f7 c7hvf ct2qg"
                         aria-hidden="true"></div>
                    <div class="cp4zc">
                      <img class="clgwa csqag ckemv c5adh cebnw ch6f7 ce83r"
                           src="https://preview.cruip.com/tidy/images/features-home-3-03.jpg" width="342" height="342"
                           alt="News 03">
                    </div>
                    <div class="cugo1 cwbd8 c4kmg c8u3l cd7c9 cvrk6 cdx1x cdiok cn59r">
                      <svg class="c6urr cdiok cn59r" viewBox="0 0 64 64" xmlns="http://www.w3.org/2000/svg">
                        <path class="cv4pf"
                              d="M25.53 40.038c1.607-.216 3.071-.576 4.655-1.08.048-.36.288-.6.552-.624l.12.408a37.15 37.15 0 0 0 2.352-.912l.12.264c1.416-.72 2.64-1.2 3.984-2.376l.312.144c1.392-1.248 1.632-2.904 1.632-4.728-.624-.912-1.416-1.656-2.784-2.112.36-.72.768-1.752.984-2.784-.12-.648-.408-1.224-.864-1.776-.84-.072-2.088-.24-3.264-.24l-.192-.216a18.485 18.485 0 0 0-1.152-.048c-1.776 0-4.056 1.032-4.056 1.944 0 .624.048 1.248.192 1.824l.268-.172c.578-.368 1.127-.671 1.46-.38l-1.656.792c.048.144.12.336.192.48 1.296-.672 3.96-1.608 5.64-1.608-.456.984-2.376 2.496-3.672 2.832l-.24 1.056c.456 1.248.864 1.032 2.16 1.68l.12-.288c1.8.216 3.336 0 3.96.72-.312 1.464-3.984 2.712-5.4 3.12-.504.144-.84.144-.936-.096-1.416.744-3.36.696-5.064.696-.24.768-.336 1.608.048 2.544l.72-.312c.144.288-.432.696-.456.96-.024.24.12.312.264.288Zm7.703-2.352-.144-.264.744-.312.072.216-.672.36Zm-4.344 1.248-.048-.264c.216-.048.384-.096.552-.12a.588.588 0 0 1 .48.12l-.984.264Z"></path>
                      </svg>
                    </div>
                  </a>
                  <h3 class="c4ryg chiic cv4op">
                    <a class="cic5i cbepq cpn01" href="#0">Advanced Features</a>
                  </h3>
                  <p class="csmmp cg9j4">Lorem ipsum is placeholder text used in the graphic, print, and publishing for
                    previewing layouts.</p>
                </article>

              </div>

            </div>
          </div>
        </section>

        <!-- Target -->
        <section>
          <div class="cwq08 cui38 cc4l3 cucgo">
            <div class="c3elr c65y5 cv2nt c4m2n">

              <!-- Section header -->
              <div class="csxy5 cquxk c54e1 cc4l3 cz6lp">
                <h2 class="c4ryg cpn01 ci9ig cgxhh">We're experts and brand creators</h2>
                <p class="csmmp csj8k">Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia
                  deserunt mollit anim id est laborum — semper quis lectus nulla at volutpat diam ut venenatis.</p>
              </div>

              <!-- Section content -->
              <div class="xl:space-x-18 cl21a ck0zt comxp c8n8h cevdo c4nar co8zu c04nu cz9ju chg82 cc4l3 cmxqt">

                <!-- Content -->
                <div class="c218p cvbuf cz9zg c3ira aos-init aos-animate" data-aos="fade-right">
                  <ul class="cygcn">
                    <li>
                      <div class="cpccj cc3ji cmxqt">
                        <svg class="cchnu c6urr c3r53 cu96n cmvs9 cua0z">
                          <path
                              d="M15.722 4.008C14.408 1.214 10.954-.635 7.318.203 5.6.596 4.072 1.561 2.919 2.757A10.57 10.57 0 0 0 .484 6.93C.03 8.458-.173 10.035.18 11.764c.191.862.518 1.683 1.146 2.479a4.876 4.876 0 0 0 2.256 1.522c1.635.469 3.156.192 4.41-.439 1.242-.615 2.298-1.769 2.494-3.094.094-.656-.537-.657-.69-.18-.781 2.126-3.715 2.534-5.265 1.579-1.568-.922-1.185-3.068-.294-4.801.89-1.729 2.454-3.02 3.92-3.338.376-.098.714-.121 1.026-.098.324.018.658.074.98.188.65.2 1.23.591 1.618 1 .27.3.575.386 1.002.461.436.061.95.117 1.499.045.535-.073 1.06-.287 1.41-.807.345-.504.462-1.348.03-2.273"></path>
                        </svg>
                        <div class="c4ryg cpn01 cgxhh">79%</div>
                      </div>
                      <div class="csmmp cg9j4">Lorem ipsum is placeholder text used in the graphic, print, and
                        publishing for previewing layouts.
                      </div>
                    </li>
                    <li>
                      <div class="cpccj cc3ji cmxqt">
                        <svg class="c1cge c6urr c3r53 cu96n cmvs9 cua0z">
                          <path
                              d="M15.722 4.008C14.408 1.214 10.954-.635 7.318.203 5.6.596 4.072 1.561 2.919 2.757A10.57 10.57 0 0 0 .484 6.93C.03 8.458-.173 10.035.18 11.764c.191.862.518 1.683 1.146 2.479a4.876 4.876 0 0 0 2.256 1.522c1.635.469 3.156.192 4.41-.439 1.242-.615 2.298-1.769 2.494-3.094.094-.656-.537-.657-.69-.18-.781 2.126-3.715 2.534-5.265 1.579-1.568-.922-1.185-3.068-.294-4.801.89-1.729 2.454-3.02 3.92-3.338.376-.098.714-.121 1.026-.098.324.018.658.074.98.188.65.2 1.23.591 1.618 1 .27.3.575.386 1.002.461.436.061.95.117 1.499.045.535-.073 1.06-.287 1.41-.807.345-.504.462-1.348.03-2.273"></path>
                        </svg>
                        <div class="c4ryg cpn01 cgxhh">1M+</div>
                      </div>
                      <div class="csmmp cg9j4">Lorem ipsum is placeholder text used in the graphic, print, and
                        publishing for previewing layouts.
                      </div>
                    </li>
                    <li>
                      <div class="cpccj cc3ji cmxqt">
                        <svg class="cqpxl c6urr c3r53 cu96n cmvs9 cua0z">
                          <path
                              d="M15.722 4.008C14.408 1.214 10.954-.635 7.318.203 5.6.596 4.072 1.561 2.919 2.757A10.57 10.57 0 0 0 .484 6.93C.03 8.458-.173 10.035.18 11.764c.191.862.518 1.683 1.146 2.479a4.876 4.876 0 0 0 2.256 1.522c1.635.469 3.156.192 4.41-.439 1.242-.615 2.298-1.769 2.494-3.094.094-.656-.537-.657-.69-.18-.781 2.126-3.715 2.534-5.265 1.579-1.568-.922-1.185-3.068-.294-4.801.89-1.729 2.454-3.02 3.92-3.338.376-.098.714-.121 1.026-.098.324.018.658.074.98.188.65.2 1.23.591 1.618 1 .27.3.575.386 1.002.461.436.061.95.117 1.499.045.535-.073 1.06-.287 1.41-.807.345-.504.462-1.348.03-2.273"></path>
                        </svg>
                        <div class="c4ryg cpn01 cgxhh">500K</div>
                      </div>
                      <div class="csmmp cg9j4">Lorem ipsum is placeholder text used in the graphic, print, and
                        publishing for previewing layouts.
                      </div>
                    </li>
                  </ul>
                </div>

                <!-- Image -->
                <div class="cri0v cz9zg aos-init aos-animate" data-aos="fade-left">
                  <img class="comxp cc4l3" src="https://preview.cruip.com/tidy/images/target.png" width="540"
                       height="540" alt="Target">
                </div>

              </div>

            </div>
          </div>
        </section>

        <!-- Pricing -->
        <section class="ctd17">

          <!-- Dark background -->
          <div class="cdw1p chtks c9y7y cd7c9 c7hvf cn574 ct2qg" aria-hidden="true"></div>

          <div class="cwq08 ctd17 cui38 cc4l3 cucgo">
            <div class="c65y5 c4m2n">

              <!-- Section header -->
              <div class="csxy5 cquxk cc4l3 cz6lp">
                <h2 class="c4ryg cy7k1 cgxhh">Find the right plan for your business</h2>
              </div>

              <!-- Pricing tables -->
              <div x-data="{ annual: true }">

                <!-- Pricing toggle -->
                <div class="cni8m corxt cpccj cvz9z c75bi cmxqt">
                  <div class="c5gki csmmp cy5nw crg4s c35dk">Pay Monthly</div>
                  <div class="form-switch c3r53">
                    <input type="checkbox" id="toggle" class="ctg7a" x-model="annual">
                    <label class="cafxj" for="toggle">
                      <span class="ck8gg cvzrw ci41p" aria-hidden="true"></span>
                      <span class="ctg7a">Pay annually</span>
                    </label>
                  </div>
                  <div class="c5gki csmmp cy5nw c35dk">Pay Yearly <span class="c0x2x">(-20%)</span></div>
                </div>

                <div class="cy425 cdby5 caw9y cns8h coqeb cc4l3 c78e1 cv19t cmejf">

                  <!-- Pricing table 1 -->
                  <div class="ciufj ctd17 chg82 cj439 ctmo0 cmxqt cpef5 cl1oi aos-init aos-animate" data-aos="fade-up">
                    <div class="c3elr cfqxn cc3ji c55zd">
                      <div class="cpn01 ck3uh cg9j4 cp0cj">Essential</div>
                      <div class="czy2k c4psy ci9ig">
                        <span class="csmmp cy5nw cq8sc">$</span>
                        <span x-text="annual ? '49' : '55'" class="c4ryg cpn01 cgv61 cgxhh">49</span>
                        <span class="c20g7 cy5nw">/mo</span>
                      </div>
                      <div class="csmmp">Better insights for growing businesses that want more customers.</div>
                    </div>
                    <div class="cy5nw ci9ig">Features include:</div>
                    <ul class="csmmp c0s3r cq2c1 cymr7">
                      <li class="cpccj cmxqt">
                        <svg class="c0x2x c6urr c3r53 cu96n cy8g3 cg1yg" viewBox="0 0 12 12"
                             xmlns="http://www.w3.org/2000/svg">
                          <path
                              d="M10.28 2.28L3.989 8.575 1.695 6.28A1 1 0 00.28 7.695l3 3a1 1 0 001.414 0l7-7A1 1 0 0010.28 2.28z"></path>
                        </svg>
                        <span>50 Placeholder text commonly</span>
                      </li>
                      <li class="cpccj cmxqt">
                        <svg class="c0x2x c6urr c3r53 cu96n cy8g3 cg1yg" viewBox="0 0 12 12"
                             xmlns="http://www.w3.org/2000/svg">
                          <path
                              d="M10.28 2.28L3.989 8.575 1.695 6.28A1 1 0 00.28 7.695l3 3a1 1 0 001.414 0l7-7A1 1 0 0010.28 2.28z"></path>
                        </svg>
                        <span>Consectetur adipiscing elit</span>
                      </li>
                      <li class="cpccj cmxqt">
                        <svg class="c0x2x c6urr c3r53 cu96n cy8g3 cg1yg" viewBox="0 0 12 12"
                             xmlns="http://www.w3.org/2000/svg">
                          <path
                              d="M10.28 2.28L3.989 8.575 1.695 6.28A1 1 0 00.28 7.695l3 3a1 1 0 001.414 0l7-7A1 1 0 0010.28 2.28z"></path>
                        </svg>
                        <span>Excepteur sint occaecat cupidatat</span>
                      </li>
                      <li class="cpccj cmxqt">
                        <svg class="c0x2x c6urr c3r53 cu96n cy8g3 cg1yg" viewBox="0 0 12 12"
                             xmlns="http://www.w3.org/2000/svg">
                          <path
                              d="M10.28 2.28L3.989 8.575 1.695 6.28A1 1 0 00.28 7.695l3 3a1 1 0 001.414 0l7-7A1 1 0 0010.28 2.28z"></path>
                        </svg>
                        <span>Officia deserunt mollit anim</span>
                      </li>
                    </ul>
                    <div class="cu64i ct7bo cgc3a">
                      <a class="cly6v cd857 cv4pf cynr0 ce83r cuuxz" href="#0">
                        Start free trial <span class="co5k7 cgu87 cs01c c6wde cgylk czxk3 coc2c">-&gt;</span>
                      </a>
                    </div>
                  </div>

                  <!-- Pricing table 2 -->
                  <div class="ciufj ctd17 chg82 cj439 ctmo0 cmxqt cpef5 cl1oi aos-init aos-animate" data-aos="fade-up"
                       data-aos-delay="100">
                    <div class="cd7c9 csdza cvl5e cbdcv cargj">
                      <div class="cmwqk cyfgy ck3uh c4kmg c4psy c35dk cuy8x c3tf4">Most Popular</div>
                    </div>
                    <div class="c3elr cfqxn cc3ji c55zd">
                      <div class="cpn01 ck3uh cg9j4 cp0cj">Premium</div>
                      <div class="czy2k c4psy ci9ig">
                        <span class="csmmp cy5nw cq8sc">$</span>
                        <span x-text="annual ? '79' : '85'" class="c4ryg cpn01 cgv61 cgxhh">79</span>
                        <span class="c20g7 cy5nw">/mo</span>
                      </div>
                      <div class="csmmp">Better insights for growing businesses that want more customers.</div>
                    </div>
                    <div class="cy5nw ci9ig">All features of Essential plus:</div>
                    <ul class="csmmp c0s3r cq2c1 cymr7">
                      <li class="cpccj cmxqt">
                        <svg class="c0x2x c6urr c3r53 cu96n cy8g3 cg1yg" viewBox="0 0 12 12"
                             xmlns="http://www.w3.org/2000/svg">
                          <path
                              d="M10.28 2.28L3.989 8.575 1.695 6.28A1 1 0 00.28 7.695l3 3a1 1 0 001.414 0l7-7A1 1 0 0010.28 2.28z"></path>
                        </svg>
                        <span>100 placeholder text commonly</span>
                      </li>
                      <li class="cpccj cmxqt">
                        <svg class="c0x2x c6urr c3r53 cu96n cy8g3 cg1yg" viewBox="0 0 12 12"
                             xmlns="http://www.w3.org/2000/svg">
                          <path
                              d="M10.28 2.28L3.989 8.575 1.695 6.28A1 1 0 00.28 7.695l3 3a1 1 0 001.414 0l7-7A1 1 0 0010.28 2.28z"></path>
                        </svg>
                        <span>Consectetur adipiscing elit</span>
                      </li>
                      <li class="cpccj cmxqt">
                        <svg class="c0x2x c6urr c3r53 cu96n cy8g3 cg1yg" viewBox="0 0 12 12"
                             xmlns="http://www.w3.org/2000/svg">
                          <path
                              d="M10.28 2.28L3.989 8.575 1.695 6.28A1 1 0 00.28 7.695l3 3a1 1 0 001.414 0l7-7A1 1 0 0010.28 2.28z"></path>
                        </svg>
                        <span>Excepteur sint occaecat cupidatat</span>
                      </li>
                      <li class="cpccj cmxqt">
                        <svg class="c0x2x c6urr c3r53 cu96n cy8g3 cg1yg" viewBox="0 0 12 12"
                             xmlns="http://www.w3.org/2000/svg">
                          <path
                              d="M10.28 2.28L3.989 8.575 1.695 6.28A1 1 0 00.28 7.695l3 3a1 1 0 001.414 0l7-7A1 1 0 0010.28 2.28z"></path>
                        </svg>
                        <span>Officia deserunt mollit anim</span>
                      </li>
                      <li class="cpccj cmxqt">
                        <svg class="c0x2x c6urr c3r53 cu96n cy8g3 cg1yg" viewBox="0 0 12 12"
                             xmlns="http://www.w3.org/2000/svg">
                          <path
                              d="M10.28 2.28L3.989 8.575 1.695 6.28A1 1 0 00.28 7.695l3 3a1 1 0 001.414 0l7-7A1 1 0 0010.28 2.28z"></path>
                        </svg>
                        <span>Placeholder text commonly used</span>
                      </li>
                    </ul>
                    <div class="cu64i ct7bo cgc3a">
                      <a class="cly6v cd857 cv4pf cynr0 ce83r cuuxz" href="#0">
                        Start free trial <span class="co5k7 cgu87 cs01c c6wde cgylk czxk3 coc2c">-&gt;</span>
                      </a>
                    </div>
                  </div>

                  <!-- Pricing table 3 -->
                  <div class="ciufj ctd17 chg82 cj439 ctmo0 cmxqt cpef5 cl1oi aos-init aos-animate" data-aos="fade-up"
                       data-aos-delay="200">
                    <div class="c3elr cfqxn cc3ji c55zd">
                      <div class="cpn01 ck3uh cg9j4 cp0cj">Advanced</div>
                      <div class="czy2k c4psy ci9ig">
                        <span class="csmmp cy5nw cq8sc">$</span>
                        <span x-text="annual ? '129' : '135'" class="c4ryg cpn01 cgv61 cgxhh">129</span>
                        <span class="c20g7 cy5nw">/mo</span>
                      </div>
                      <div class="csmmp">Better insights for growing businesses that want more customers.</div>
                    </div>
                    <div class="cy5nw ci9ig">All features of Essential plus:</div>
                    <ul class="csmmp c0s3r cq2c1 cymr7">
                      <li class="cpccj cmxqt">
                        <svg class="c0x2x c6urr c3r53 cu96n cy8g3 cg1yg" viewBox="0 0 12 12"
                             xmlns="http://www.w3.org/2000/svg">
                          <path
                              d="M10.28 2.28L3.989 8.575 1.695 6.28A1 1 0 00.28 7.695l3 3a1 1 0 001.414 0l7-7A1 1 0 0010.28 2.28z"></path>
                        </svg>
                        <span>200 placeholder text commonly</span>
                      </li>
                      <li class="cpccj cmxqt">
                        <svg class="c0x2x c6urr c3r53 cu96n cy8g3 cg1yg" viewBox="0 0 12 12"
                             xmlns="http://www.w3.org/2000/svg">
                          <path
                              d="M10.28 2.28L3.989 8.575 1.695 6.28A1 1 0 00.28 7.695l3 3a1 1 0 001.414 0l7-7A1 1 0 0010.28 2.28z"></path>
                        </svg>
                        <span>Consectetur adipiscing elit</span>
                      </li>
                      <li class="cpccj cmxqt">
                        <svg class="c0x2x c6urr c3r53 cu96n cy8g3 cg1yg" viewBox="0 0 12 12"
                             xmlns="http://www.w3.org/2000/svg">
                          <path
                              d="M10.28 2.28L3.989 8.575 1.695 6.28A1 1 0 00.28 7.695l3 3a1 1 0 001.414 0l7-7A1 1 0 0010.28 2.28z"></path>
                        </svg>
                        <span>Excepteur sint occaecat cupidatat</span>
                      </li>
                      <li class="cpccj cmxqt">
                        <svg class="c0x2x c6urr c3r53 cu96n cy8g3 cg1yg" viewBox="0 0 12 12"
                             xmlns="http://www.w3.org/2000/svg">
                          <path
                              d="M10.28 2.28L3.989 8.575 1.695 6.28A1 1 0 00.28 7.695l3 3a1 1 0 001.414 0l7-7A1 1 0 0010.28 2.28z"></path>
                        </svg>
                        <span>Officia deserunt mollit anim</span>
                      </li>
                      <li class="cpccj cmxqt">
                        <svg class="c0x2x c6urr c3r53 cu96n cy8g3 cg1yg" viewBox="0 0 12 12"
                             xmlns="http://www.w3.org/2000/svg">
                          <path
                              d="M10.28 2.28L3.989 8.575 1.695 6.28A1 1 0 00.28 7.695l3 3a1 1 0 001.414 0l7-7A1 1 0 0010.28 2.28z"></path>
                        </svg>
                        <span>Voluptate velit esse cillum</span>
                      </li>
                      <li class="cpccj cmxqt">
                        <svg class="c0x2x c6urr c3r53 cu96n cy8g3 cg1yg" viewBox="0 0 12 12"
                             xmlns="http://www.w3.org/2000/svg">
                          <path
                              d="M10.28 2.28L3.989 8.575 1.695 6.28A1 1 0 00.28 7.695l3 3a1 1 0 001.414 0l7-7A1 1 0 0010.28 2.28z"></path>
                        </svg>
                        <span>Placeholder text commonly used</span>
                      </li>
                    </ul>
                    <div class="cu64i ct7bo cgc3a">
                      <a class="cly6v cd857 cv4pf cynr0 ce83r cuuxz" href="#0">
                        Start free trial <span class="co5k7 cgu87 cs01c c6wde cgylk czxk3 coc2c">-&gt;</span>
                      </a>
                    </div>
                  </div>

                </div>

              </div>

            </div>
          </div>
        </section>

        <!-- Cta -->
        <section class="caqoh">
          <div class="cwq08 ctd17 cui38 cc4l3 cucgo">
            <div class="c65y5 c4m2n">

              <div class="csxy5 cquxk ctd17 cc4l3">

                <div class="ck9ub cjefo cd7c9 csdza cv4f1 cbdcv chaf5" aria-hidden="true">
                  <svg class="ck9ub" width="56" height="43">
                    <path
                        d="M4.532 30.45C15.785 23.25 24.457 12.204 29.766.199c.034-.074-.246-.247-.3-.186-4.227 5.033-9.298 9.282-14.372 13.162C10 17.07 4.919 20.61.21 24.639c-1.173 1.005 2.889 6.733 4.322 5.81M18.96 42.198c12.145-4.05 24.12-8.556 36.631-12.365.076-.024.025-.349-.055-.347-6.542.087-13.277.083-19.982.827-6.69.74-13.349 2.24-19.373 5.197-1.53.75 1.252 7.196 2.778 6.688"></path>
                  </svg>
                </div>

                <div class="ctd17">
                  <h2 class="c4ryg cpn01 cc3ji cgxhh">Say goodbye to long queues, big updates, and <span class="c0x2x">confusion</span>.
                  </h2>
                  <p class="csmmp csj8k c47r3">Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia
                    deserunt mollit anim id est laborum — semper quis lectus nulla at volutpat diam ut venenatis.</p>
                  <div>
                    <a class="cly6v cd857 cv4pf cuuxz cy3fp" href="request-demo.html">
                      Request Demo <span class="co5k7 cgu87 cs01c c6wde cgylk czxk3 coc2c">-&gt;</span>
                    </a>
                  </div>
                </div>

              </div>

            </div>
          </div>
        </section>

      </main>

      <!-- Site footer -->
      <footer>
        <div class="cwq08 cui38 cc4l3 cucgo">

          <!-- Top area: Blocks -->
          <div class="cwgoa cwxaa c78e1 cv19t cqf8y">

            <!-- 1st block -->
            <div class="cabaf c9d74 cln6f">
              <div class="chiic">
                <!-- Logo -->
                <a class="ckuoi cgylk c4psy czxk3 cebnw" href="index.html" aria-label="Cruip">
                  <svg class="c6urr cive7 cxllq" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg">
                    <path
                        d="M15.25 4.116c.039.899-.51.468-.79.629-.894.524-1.491 2.04-2.612 2.125-.423.87-1.121.898-1.874 1.503-.327.256-.463.839-.756 1.097l-3.694 3.27a2.395 2.395 0 0 1-.44.314c-.378.219-.656.717-1.096.81-.475.106-1.601-.775-2.633-2.012-.825-1.587-.025-1.924.518-2.525.916-1.022 2.48-2.064 3.585-2.753.843-.537 1.677-1.13 2.59-1.482.935-.357 1.779-.842 2.738-1.041.7-.141 1.522.063 2.206 0a9.596 9.596 0 0 1 2.258.065M30.676 3.646c-.06 1.046-1.038.955-1.593 1.363C27.32 6.31 25.8 8.656 23.63 9.583c-1.07 1.412-2.411 1.952-4.056 3.254-.711.56-1.21 1.417-1.877 1.965-2.887 2.381-5.668 4.524-8.64 6.823-.303.236-.646.468-1.008.697-.834.528-1.675 1.394-2.543 1.77-.95.413-2.376-.279-3.375-1.544-.43-1.849 1.112-2.657 2.38-3.737 2.13-1.82 5.33-4.012 7.558-5.536 1.707-1.17 3.395-2.426 5.138-3.43 1.789-1.03 3.439-2.179 5.224-3.063 1.303-.643 2.758-.96 4.038-1.53a40.762 40.762 0 0 1 4.207-1.606M30.386 14.346c.229.918-.566.8-.896 1.136-1.048 1.058-1.721 3.056-3.254 3.7-.563 1.17-1.522 1.532-2.603 2.507-.464.426-.731 1.128-1.177 1.542-1.94 1.77-3.91 3.263-6.082 4.772a6.36 6.36 0 0 1-.748.43c-.618.313-1.24.914-1.901 1.065-.731.161-1.856-.807-2.662-2.199-.401-1.784.715-2.129 1.6-2.818 1.49-1.15 3.693-2.49 5.192-3.486 1.154-.755 2.247-1.633 3.417-2.292 1.2-.68 2.244-1.52 3.44-2.128.868-.448 1.927-.61 2.79-1.029.92-.447 1.873-.85 2.884-1.2"></path>
                  </svg>
                </a>
              </div>
              <div class="cpn01 c1stc cg9j4">The smarter way to start your next idea.</div>
            </div>

            <!-- 2nd block -->
            <div class="cm13t ct8yv ci5yk">
              <h6 class="cpn01 ck3uh c35dk chiic">How it works</h6>
              <ul class="cy5nw crwlr c35dk">
                <li>
                  <a class="cjtfg csmmp cgylk czxk3 cebnw" href="#0">Overview</a>
                </li>
                <li>
                  <a class="cjtfg csmmp cgylk czxk3 cebnw" href="#0">Pricing</a>
                </li>
                <li>
                  <a class="cjtfg csmmp cgylk czxk3 cebnw" href="#0">Service Areas</a>
                </li>
              </ul>
            </div>

            <!-- 3rd block -->
            <div class="cm13t ct8yv ci5yk">
              <h6 class="cpn01 ck3uh c35dk chiic">Resources</h6>
              <ul class="cy5nw crwlr c35dk">
                <li>
                  <a class="cjtfg csmmp cgylk czxk3 cebnw" href="#0">Customer Stories</a>
                </li>
                <li>
                  <a class="cjtfg csmmp cgylk czxk3 cebnw" href="#0">Knowledge Base</a>
                </li>
                <li>
                  <a class="cjtfg csmmp cgylk czxk3 cebnw" href="#0">Contact Us</a>
                </li>
              </ul>
            </div>

            <!-- 4th block -->
            <div class="cm13t ct8yv ci5yk">
              <h6 class="cpn01 ck3uh c35dk chiic">Products</h6>
              <ul class="cy5nw crwlr c35dk">
                <li>
                  <a class="cjtfg csmmp cgylk czxk3 cebnw" href="#0">Corporate Partners</a>
                </li>
                <li>
                  <a class="cjtfg csmmp cgylk czxk3 cebnw" href="#0">Secure Identity</a>
                </li>
                <li>
                  <a class="cjtfg csmmp cgylk czxk3 cebnw" href="#0">Legal Help</a>
                </li>
                <li>
                  <a class="cjtfg csmmp cgylk czxk3 cebnw" href="#0">First Capital</a>
                </li>
              </ul>
            </div>

            <!-- 5th block -->
            <div class="cm13t ct8yv ci5yk">
              <h6 class="cpn01 ck3uh c35dk chiic">Company</h6>
              <ul class="cy5nw crwlr c35dk">
                <li>
                  <a class="cjtfg csmmp cgylk czxk3 cebnw" href="#0">About Us</a>
                </li>
                <li>
                  <a class="cjtfg csmmp cgylk czxk3 cebnw" href="#0">Careers</a>
                </li>
                <li>
                  <a class="cjtfg csmmp cgylk czxk3 cebnw" href="#0">Terms of Use</a>
                </li>
              </ul>
            </div>

          </div>

          <!-- Bottom area -->
          <div class="cnpdp c3elr cl21a cv2nt csvbf c140r cgodi">

            <!-- Social links -->
            <ul class="czwqv ckmjp cn3fl c5ud2 cc3ji cmxqt">
              <li>
                <a class="cjtfg cchnu cgylk czxk3 cebnw" href="#0" aria-label="Twitter">
                  <svg class="c6urr c3qv0 culew" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
                    <path
                        d="m6.329 1 4.369 5.594L15.75 1h3.068L12.12 8.414 20 18.5h-6.172l-4.833-6.116L3.464 18.5H.395l7.169-7.928L0 1h6.329Zm-.925 1.684H3.583l11.093 14.04h1.7L5.404 2.684Z"></path>
                  </svg>
                </a>
              </li>
              <li>
                <a class="cjtfg cchnu cgylk czxk3 cebnw" href="#0" aria-label="Facebook">
                  <svg class="c6urr c3qv0 culew" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
                    <path
                        d="M20 10.025C20 4.491 15.52 0 10 0S0 4.491 0 10.025c0 4.852 3.44 8.892 8 9.825v-6.817H6v-3.008h2V7.52a3.508 3.508 0 0 1 3.5-3.509H14v3.008h-2c-.55 0-1 .45-1 1.002v2.005h3v3.008h-3V20c5.05-.501 9-4.772 9-9.975Z"></path>
                  </svg>
                </a>
              </li>
              <li>
                <a class="cjtfg cchnu cgylk czxk3 cebnw" href="#0" aria-label="Telegram">
                  <svg class="c6urr c3qv0 culew" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
                    <path
                        d="M19.96 2.336a.421.421 0 0 0-.291-.308 1.543 1.543 0 0 0-.788.054S1.358 8.194.358 8.87c-.215.145-.288.23-.324.33-.173.485.366.694.366.694l4.517 1.428a.506.506 0 0 0 .229-.013c1.026-.63 10.332-6.335 10.873-6.527.083-.024.148 0 .131.061-.215.732-8.257 7.664-8.301 7.706a.16.16 0 0 0-.06.143l-.422 4.28s-.176 1.331 1.196 0a38.082 38.082 0 0 1 2.374-2.11c1.553 1.041 3.224 2.192 3.945 2.794.245.23.576.354.916.342.426-.05.774-.35.876-.754 0 0 3.192-12.471 3.298-14.142.011-.162.025-.268.027-.38.005-.13-.008-.26-.04-.387Z"></path>
                  </svg>
                </a>
              </li>
              <li>
                <a class="cjtfg cchnu cgylk czxk3 cebnw" href="#0" aria-label="Github">
                  <svg class="c6urr c3qv0 culew" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
                    <path
                        d="M10.041 0C4.52 0 0 4.612 0 10.25c0 4.526 2.845 8.37 6.862 9.737.502.085.669-.257.669-.513v-1.708c-2.761.598-3.347-1.367-3.347-1.367-.419-1.196-1.088-1.537-1.088-1.537-1.004-.598 0-.598 0-.598 1.004.085 1.506 1.025 1.506 1.025.92 1.537 2.343 1.11 2.929.854.084-.683.335-1.11.67-1.367-2.26-.256-4.603-1.11-4.603-5.039 0-1.11.419-2.05 1.004-2.733 0-.342-.418-1.367.168-2.733 0 0 .836-.257 2.76 1.025.838-.257 1.674-.342 2.511-.342.837 0 1.674.085 2.51.342 1.925-1.367 2.762-1.025 2.762-1.025.586 1.452.167 2.477.084 2.733.669.683 1.004 1.623 1.004 2.733 0 3.93-2.343 4.783-4.603 5.04.335.341.67.939.67 1.879v2.818c0 .256.167.598.67.513 4.016-1.367 6.86-5.21 6.86-9.737C20.084 4.612 15.565 0 10.042 0Z"></path>
                  </svg>
                </a>
              </li>
            </ul>

            <!-- Copyrights note -->
            <div class="csmmp c35dk cb6q3">© Cruip.com. All rights reserved.</div>

          </div>

        </div>
      </footer>

    </div>

    <script src="./js/vendors/alpinejs.min.js" defer=""></script>
    <script src="./js/vendors/aos.js"></script>
    <script src="./js/main.js"></script>


    <script>console.log("%cImportant!", "color: blue; font-size: x-large");
    console.log("%cThe page you are viewing is for demo purposes only. CSS and HTML have been minified and class names have been shortened to improve the page load time. Download our templates from https://cruip.com/ 😉", "font-size: large");</script>
    <script>const pagesList = [{
      "name": "Home",
      "url": "https://preview.cruip.com/tidy/index.html",
      "active": true
    }, {"name": "Pricing", "url": "https://preview.cruip.com/tidy/pricing.html", "active": false}, {
      "name": "About",
      "url": "https://preview.cruip.com/tidy/about.html",
      "active": false
    }, {"name": "Blog", "url": "https://preview.cruip.com/tidy/blog.html", "active": false}, {
      "name": "Blog Post",
      "url": "https://preview.cruip.com/tidy/blog-post.html",
      "active": false
    }, {
      "name": "Wall of Love",
      "url": "https://preview.cruip.com/tidy/wall-of-love.html",
      "active": false
    }, {
      "name": "Wall of Love Post",
      "url": "https://preview.cruip.com/tidy/wall-of-love-single.html",
      "active": false
    }, {"name": "404", "url": "https://preview.cruip.com/tidy/404.html", "active": false}, {
      "name": "Support",
      "url": "https://preview.cruip.com/tidy/support.html",
      "active": false
    }, {
      "name": "Sign in",
      "url": "https://preview.cruip.com/tidy/signin.html",
      "active": false
    }, {
      "name": "Reset password",
      "url": "https://preview.cruip.com/tidy/reset-password.html",
      "active": false
    }, {"name": "Request Demo", "url": "https://preview.cruip.com/tidy/request-demo.html", "active": false}];
    if (window != top) {
      window.parent.postMessage(pagesList, "https://cruip.com")
    }
    ;</script>
    <script defer=""
            src="https://static.cloudflareinsights.com/beacon.min.js/vcd15cbe7772f49c399c6a5babf22c1241717689176015"
            integrity="sha512-ZpsOmlRQV6y907TI0dKBHq9Md29nnaEIPlkf84rnaERnq6zvWvPUqr2ft8M1aS28oN72PdrCzSjY4U6VaAw1EQ=="
            data-cf-beacon="{&quot;rayId&quot;:&quot;8d4db40a089e84f7&quot;,&quot;version&quot;:&quot;2024.10.1&quot;,&quot;r&quot;:1,&quot;token&quot;:&quot;59cc17d45d734f9ba118c63036ab1b84&quot;,&quot;serverTiming&quot;:{&quot;name&quot;:{&quot;cfExtPri&quot;:true,&quot;cfL4&quot;:true,&quot;cfSpeedBrain&quot;:true,&quot;cfCacheStatus&quot;:true}}}"
            crossorigin="anonymous"></script>
  </div>
</template>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>