<script>
	import { page } from '@roxi/routify';
	$: {
		if (typeof gtag !== "undefined"){
			gtag("config", "UA-SOMEANALYTICSID-1", {
				page_path: $page.path
			});
		}
	}
</script>
