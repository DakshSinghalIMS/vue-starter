<template>
	<div style="margin-top: 125px;">
        <!-- Push Footer -->
    </div>
    <footer class="footer">
        <div class="container" style="color: #777;">
            <!-- Company Information -->
            <div class="pull-left" style="padding-top: 28px;">
                Copyright &copy; Yourname - <a v-link="{ path: '/terms'}">Terms Of Service</a>
            </div>
            <!-- Social Icons -->
            <div class="pull-right footer-social-icons">
                <a href="http://facebook.com/{{ links.facebook }}">
                    <i class="fa fa-btn fa-facebook-square"></i>
                </a>
                <a href="http://twitter.com/{{ links.twitter }}">
                    <i class="fa fa-btn fa-twitter-square"></i>
                </a>
                <a href="http://github.com/{{ links.github }}">
                    <i class="fa fa-github-square"></i>
                </a>
            </div>
            <div class="clearfix"></div>
        </div>
    </footer>
</template>

<script>
module.exports = {
    data: function () {
        return {
            links: {
            	facebook: '',
            	twitter: '',
            	github: ''
            }
        }
    }
}
</script>