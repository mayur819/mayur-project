In this it icludes all-
a. A fixed navbar that does not move when scrolling.
b. Below the navbar, create three sections: a left menu, a main content area,
and a right-side panel.
c. Include a footer at the bottom.
d. Make the left menu collapsible.


And the java function for the screen width is -
 function adjustPageSize() {
            const screenWidth = window.innerWidth;
            const body = document.body;

            if (screenWidth >= 992 && screenWidth <= 1600) {
                body.style.transform = 'scale(0.9)';
                body.style.transformOrigin = 'top left';
            } else if (screenWidth >= 700 && screenWidth <= 767) {
                body.style.transform = 'scale(0.8)';
                body.style.transformOrigin = 'top left';
            } else if (screenWidth >= 600 && screenWidth < 700) {
                body.style.transform = 'scale(0.75)';
                body.style.transformOrigin = 'top left';
            } else if (screenWidth <= 600) {
                body.style.transform = 'scale(0.5)';
                body.style.transformOrigin = 'top left';
            } else {
                body.style.transform = 'scale(1)';
            }
        }

        window.addEventListener('resize', adjustPageSize);
        window.addEventListener('load', adjustPageSize);
    </script>
</body>
</html>
