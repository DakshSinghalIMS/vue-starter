<template></template>

<script>
module.exports = {

	route: {
		activate: function (transition) {
			this.$root.authenticated = false;
			this.$root.user = null;
			localStorage.removeItem('user');
			localStorage.removeItem('token');
			transition.redirect('/');
		}
	}
}
</script>