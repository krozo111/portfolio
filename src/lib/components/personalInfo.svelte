<script>
  import { personalInfo } from "$lib/config";
  import Icon from "@iconify/svelte";
</script>

<div class="px-5 py-5 mt-5 rounded-2xl bg-surface-50 dark:bg-surface-900">
  <div class="flex border-b pb-2.5">
    <span class="">
      <Icon icon="streamline-emojis:telephone" width="36" />
    </span>
    <div class="text-left ml-2.5">
      <p class="text-xs text-surface-300">Phone</p>
      <p class="">{personalInfo.phone}</p>
    </div>
  </div>
  <div class="flex border-b py-2.5">
    <span class="socialbtnshadow-md">
      <Icon icon="streamline-emojis:open-mailbox-with-raised-flag" width="36" />
    </span>
    <div class="text-left ml-2.5">
      <p class="text-xs text-surface-300">Email</p>
      <p class="">{personalInfo.email}</p>
    </div>
  </div>
  <div class="flex border-b py-2.5">
    <span class="">
      <Icon icon="streamline-emojis:australia" width="36" />
    </span>
    <div class="text-left ml-2.5">
      <p class="text-xs text-surface-300">Location</p>
      <p class="">{personalInfo.location}</p>
    </div>
  </div>
  <div class="flex py-2.5">
    <span class="">
      <Icon icon="streamline-emojis:birthday-cake-1" width="36" />
    </span>
    <div class="text-left ml-2.5">
      <p class="text-xs text-surface-300">Birthday</p>
      <p class="">{personalInfo.dob}</p>
    </div>
  </div>
</div>
