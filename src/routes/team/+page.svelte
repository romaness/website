<script lang="ts">
	import { base } from '$app/paths';
	import InfoBox from '$lib/layout/InfoBox.svelte';
	import PageLayout from '$lib/layout/PageLayout.svelte';
	import joern from './joern.jpg';
	import marco from './marco.jpg';
	import robert from './robert.png';
	import TeamMember from './TeamMember.svelte';
	import TeamMemberSection from './TeamMemberSection.svelte';
	import wolfram from './wolfram.jpg';
</script>

<PageLayout>
	<h1>The Team</h1>
	<InfoBox title="Who are we?">
		<p>
			We are simple developers organizing this event in our spare time. If you have any questions or
			problems before or during the conference, don't hesitate to contact one of us!
		</p>
		<p>
			Throughout the years, there were lots of people involved in organizing the past events. You
			can <a href="{base}/team/alumni">find out more about our alumnis on the /team/alumni page</a>.
		</p>
	</InfoBox>

	<p>
		You can always reach us by e-mail: <a href="mailto:team@jscraftcamp.org">team@jscraftcamp.org</a
		>
	</p>

	<TeamMemberSection>
		<TeamMember name="Bernd Kaiser" />
		<TeamMember name="Gustaf Graf" />
		<TeamMember image={joern} name="Jörn Bernhardt" email="joern.bernhardt@compose.us" />
		<TeamMember image={marco} name="Marco Emrich" email="marco.emrich@codecentric.de" />
		<TeamMember name="Philip Saa" />
		<TeamMember image={robert} name="Robert Hostlowsky" />
		<TeamMember image={wolfram} name="Wolfram Kriesing" email="w@kriesing.de" />
	</TeamMemberSection>

	<p>
		Want to see yourself on the list and help out? <a href="https://discord.gg/3mHhaXVEjP"
			>Join our Discord and the regular orga meetings</a
		>!
	</p>
</PageLayout>
