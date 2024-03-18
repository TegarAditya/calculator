<script>
	import { Navbar, NavBrand, NavLi, NavUl, NavHamburger } from 'flowbite-svelte';
	import { Button } from 'flowbite-svelte';
	import { LightbulbSolid } from 'flowbite-svelte-icons';
	import '../app.pcss';
</script>

<div class="flex h-[100dvh] justify-center">
	<div class="mx-auto w-screen max-w-md flex-col justify-between">
		<Navbar class="fixed">
			<NavBrand href="/" class="py-2">
				<span class="self-center whitespace-nowrap text-xl font-semibold dark:text-white"
					>Simple Calc</span
				>
			</NavBrand>
			<div class="flex align-middle space-x-2">
				<Button class="!p-2 w-10 h-10" color="light" size="xl" href="/">
					<LightbulbSolid class="h-4 w-4 text-gray-600 dark:text-gray-400" />
				</Button>
			</div>
		</Navbar>
		<slot />
	</div>
</div>
