<template>
    <div id="skills">
        <div id="right-info">
            <div class="container">
                <div class="skills" role="alert">
                    <ul>
                        <li>{{ l1 }}</li>
                        <li>{{ l2 }}</li>
                        <li>{{ l3 }}</li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'skills',
    data () {
        return {
            l1: 'HTML',
            l2: 'Python',
            l3: 'Java',

        }
    }
}
</script>