<template>
  <div class="image bg-gray-100 rounded w-full">
        <div class="flex justify-center flex-col items-center p-4">
          <img
            src="data:image/jpeg;base64,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"
            alt=""
            class="
              rounded-full
              w-36
              h-36
              -mt-14
              border border-gray-100
              shadow-xl
            "
          />
          <div class="rounded-xl flex bg-white mt-2 py-1 px-2 items-center">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="h-4 w-4 mx-1"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
              stroke-width="2"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                d="M15.232 5.232l3.536 3.536m-2.036-5.036a2.5 2.5 0 113.536 3.536L6.5 21.036H3v-3.572L16.732 3.732z"
              />
            </svg>
            <span>تغيير الصورة</span>
          </div>
          <div class="text-center py-2">
            <h2>احمد عادل محمد</h2>
          </div>
        </div>
      </div>
</template>

<script>
export default {
name:"ProfileHeader"
}
</script>

<style>

</style>