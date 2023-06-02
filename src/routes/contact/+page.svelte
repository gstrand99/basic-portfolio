<script lang="ts">
  import { Avatar } from "@skeletonlabs/skeleton";
  import { clipboard } from '@skeletonlabs/skeleton';

  const email: string = 'contact@garrett-strand.tech'
</script>

<div class="container h-full mx-auto flex justify-center items-center">
  <div class="space-y-10 text-center flex flex-col items-center">
    <div class="card p-4">
	    <section class="p-4"><Avatar src="https://ca.slack-edge.com/T03064S72JE-U04MUFP5HFH-8db8acfafaf0-512" width="w-50" rounded="rounded-full" /></section>
	    <section class="p-4">Email: contact@garrett-strand.tech  <button class="btn btn-sm variant-filled " use:clipboard={email}>Click to copy</button></section> 
    </div>
  </div>
</div>
