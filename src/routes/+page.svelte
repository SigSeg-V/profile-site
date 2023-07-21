<script lang="ts">
  import Navbar from "$lib/components/navbar.svelte";

	const myAge = () => {
		const birthday = new Date(1999, 8, 28).getTime();
		const now = Date.now();
		const diff = now - birthday;
		return new Date(diff).getUTCFullYear() - 1970;
	};
</script>

<Navbar />

<div class="flex justify-center m-5">
	<div class="sm:w-2/3 m-2">
		<div class="p-2">
			<h2 class="text-xl">About Me</h2>
			<p>
				I'm a {myAge()} year old Rust evangelist with a passion for everything software: when I am not
				writing software at my day job, I'm writing it in my own time. I started back in 2015 wanting
				to mod a little known game called Call of Duty: World at War where I struggled for 3 hours on
				ugx-mods trying to understand how to programatically open a door. Since then software has continued
				to excite me and so I always take pride in making good experiences.
			</p>
		</div>
		<div class="p-2">
			<h2 class="text-xl">Work Experience</h2>
			<ul class="list-disc ml-5">
				<li>
					BMM Test Labs — Box Hill, Vic
					<br />
					Software Engineer | Feb 2022 — Jan 2023
					<br />
					Evaluate the mathematics of various gambling games, such as card games and slot machines.
					<br />
					Write software (C++/C#) that calculates exactly the return to player (RTP) and other related
					statistics for many manufacturers’ slot machines including Konami, Aristocrat, IGT and Ainsworth.
					<br />
					Develop simulation software (C++/C#) that simulates slot machines and replicate the games’
					functions for combination testing.
				</li>
				<li>
					ANZ — Docklands, Vic
					<br />
					Software Engineer, Core Systems | Jan 2023 — Current
					<br />
					Developed API endpoints for Splunk monitoring systems and Core Accounts Processing using z/OS
					connect and Hogan.
					<br />
					As part of the DevOps team, replaced Endevor SCM with Git and CI/CD based deploy through Codefresh.
					Most notably I designed and developed a build and deploy system locally on the mainframe for
					production hotfixes.
				</li>
			</ul>
		</div>
		<div class="p-2">
			<h2 class="text-xl">Certificates and Awards</h2>
			<ul class="list-disc ml-5">
				<li>
					2023 IBM Mainframe System Operator Level I. Melbourne, Au
					<br />
				</li>
				<li>2021 Finalist, UoM Dulux award (Phys. and Theoretical Chemistry). Melbourne, Au</li>
				<li>2019 N2, Japanese Language Proficiency Test. Melbourne, Au</li>
			</ul>
		</div>
		<div class="p-2">
			<h2 class="text-xl">Education</h2>
			<ul class="list-disc ml-5">
				<li>
					University of Melbourne - Bachelor of Science (Mar. 2017 Nov. 2020)
					<br />
					Minored in Japanese language
					<br />
					Graduation project - computationally modeling the quantum magnetism of tetrahedral Co(II) complexes,
					and comparing this novel understanding of complex chemistry with the previous understanding
					of Co(II)
				</li>
				<li>
					University of Melbourne - Master of Science - incomplete (Mar. 2021 - Feb. 2022)
					<br />
					Researched the quantum effects in single ion (molecule) magnets in lanthanides and transition
					metals.
					<br />
					Picked to represent the Theoretical Chemistry department to present our research at Dulux.
				</li>
			</ul>
		</div>
	</div>
</div>
