<script>
  export let phone = "No number available";
  export let email = "No email available";
  export let location = "No location available";
  export let dob = "01-01-2000";
  import Icon from "@iconify/svelte";
</script>

<div class="px-5 py-5 mt-5 rounded-2xl bg-surface-900">
  <div class="flex border-b pb-2.5">
    <span class="">
      <Icon icon="streamline-emojis:telephone" width="36" />
    </span>
    <div class="text-left ml-2.5">
      <p class="text-xs text-surface-300">Phone</p>
      <p class="">{phone}</p>
    </div>
  </div>
  <div class="flex border-b py-2.5">
    <span class="socialbtnshadow-md">
      <Icon icon="streamline-emojis:open-mailbox-with-raised-flag" width="36" />
    </span>
    <div class="text-left ml-2.5">
      <p class="text-xs text-surface-300">Email</p>
      <p class="">{email}</p>
    </div>
  </div>
  <div class="flex border-b py-2.5">
    <span class="">
      <Icon icon="streamline-emojis:australia" width="36" />
    </span>
    <div class="text-left ml-2.5">
      <p class="text-xs text-surface-300">Location</p>
      <p class="">{location}</p>
    </div>
  </div>
  <div class="flex py-2.5">
    <span class="">
      <Icon icon="streamline-emojis:birthday-cake-1" width="36" />
    </span>
    <div class="text-left ml-2.5">
      <p class="text-xs text-surface-300">Birthday</p>
      <p class="">{dob}</p>
    </div>
  </div>
</div>
