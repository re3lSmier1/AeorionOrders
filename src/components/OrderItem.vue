<script setup lang="ts">

</script>

<template>
  <!-- Button trigger modal -->

    <a href="#" class="text-decoration-none" data-bs-toggle="modal" data-bs-target="#exampleModal">
      <div class="card p-1 py-2 text-center" style="border: #eee 1px solid;">
        <div class="text-center">
          <img src="/egg-sandwich.png" alt=""
               style="max-width: 150px; max-height: 150px; width: auto; height: auto;">
          <div style="font-weight: bold">Egg Sandwich</div>
        </div>

      </div>
    </a>


  <!-- Modal -->
  <div class="modal fade" id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true"
  >
    <div class="modal-dialog modal-lg border-0">
      <div class="modal-content">
        <div class="modal-body">
          <div >
            <div class="text-center">
              <img src="/egg-sandwich.png" alt=""
                   style="max-width: 200px; max-height: 200px; width: auto; height: auto;"/>
              <div style="font-weight: bold; font-size: 24px; color: #777">
                Egg Sandwich
              </div>
            </div>
            <br>
            <ul class="nav nav-underline" id="myTab" role="tablist">
              <li class="nav-item" role="presentation">
                <button class="nav-link active" id="home-tab" data-bs-toggle="tab" data-bs-target="#home-tab-pane" type="button" role="tab" aria-controls="home-tab-pane" aria-selected="true">Customize</button>
              </li>
              <li class="nav-item" role="presentation">
                <button class="nav-link" id="profile-tab" data-bs-toggle="tab" data-bs-target="#profile-tab-pane" type="button" role="tab" aria-controls="profile-tab-pane" aria-selected="false">Flavours</button>
              </li>
              <li class="nav-item" role="presentation">
                <button class="nav-link" id="contact-tab" data-bs-toggle="tab" data-bs-target="#contact-tab-pane" type="button" role="tab" aria-controls="contact-tab-pane" aria-selected="false">Sides</button>
              </li>

            </ul>
            <br>
            <div class="tab-content" id="myTabContent">
              <div class="tab-pane fade show active" id="home-tab-pane" role="tabpanel" aria-labelledby="home-tab" tabindex="0">
                <div class="row">
                  <div class="col-md-3">
                    <div class="text-center">
                      <img src="/fried-egg.png" alt="" style="max-width: 100px; max-height: 100px; width: auto; height: auto;">
                      <div style="font-weight: bold; margin-top: 15px">Fried Egg</div>

                    </div>
                     </div>
                </div>
              </div>
              <div class="tab-pane fade" id="profile-tab-pane" role="tabpanel" aria-labelledby="profile-tab" tabindex="0">
                Quesadilla
              </div>
              <div class="tab-pane fade" id="contact-tab-pane" role="tabpanel" aria-labelledby="contact-tab" tabindex="0">...</div>
              <div class="tab-pane fade" id="disabled-tab-pane" role="tabpanel" aria-labelledby="disabled-tab" tabindex="0">...</div>
            </div>
          </div>
        </div>
        <div class="modal-footer">
          <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
          <button type="button" class="btn btn-primary">Save changes</button>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>

</style>