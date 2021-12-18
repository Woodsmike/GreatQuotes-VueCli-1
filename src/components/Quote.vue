<template>
    <div class="col-sm-6 col-md-4 col-lg-3">
        <div class="panel panel-default">
            <div class="panel-body quote">
                <slot></slot>
            </div>
        </div>
    </div>
</template>

<script>
</script>

<style>
    
    .panel-body {
        font-family: 'Arizonia', cursive;
        font-size: 18px;
        color: #6e6e6e;
        background-color: aqua;
    }

    .quote {
        cursor: pointer;
        margin-bottom: 10px;
        min-height: 105px;
        max-height: 105px;        
        padding: 15px;
        border-radius: 10px;
    }
    .quote:hover {
        background-color: #ffe2e2;
    }
</style>