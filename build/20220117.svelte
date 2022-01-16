<script>
    export let post;
    import Template from '../_Template.svelte';
    import Tag from '../_Tag.svelte';
    import moment from 'moment';
</script>

<Template>
    <div slot="published">
        {moment(post.published).format('MMMM Do dddd, YYYY년')}
    </div>
    <div slot="title">리더가 프로젝트를 망치는 방법.</div>
    <div slot="subtitle">리더는 열심히 하는게 아닌 잘 해야하는 자리다.</div>
    <Tag slot="tag" tags={post.tag} />
    <div slot="content">
        <img class="image-1" src="https://images.unsplash.com/photo-1522071820081-009f0129c71c?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2070&q=80" alt="leader">
        <div>
            의도하던 의도하지 않았던 우리는 프로젝트가 산으로 가는 경험은 누구나 한 번 씩 겪어봤을 일이다. 의도하던 의도하지 않았던 우리는 프로젝트가 산으로 가는 경험은 누구나 한 번 씩 겪어봤을 일이다. 의도하던 의도하지 않았던 우리는 프로젝트가 산으로 가는 경험은 누구나 한 번 씩 겪어봤을 일이다. 겪어봤을 일이다.
        </div>
        <div>
            의도하던 의도하지 않았던 우리는 프로젝트가 산으로 가는 경험은 누구나 한 번 씩 겪어봤을 일이다. 의도하던 의도하지 않았던 우리는 프로젝트가 산으로 가는 경험은 누구나 한 번 씩 겪어봤을 일이다. 의도하던 의도하지 않았던 우리는 프로젝트가 산으로 가는 경험은 누구나 한 번 씩 겪어봤을 일이다.
        </div>
    </div>
</Template>

<style lang="scss">
    .image-1 {
        object-fit: cover;
        height: 360px;
    }

    @media (max-width: 768px) {
        .image-1 {
            height: 240px;
        }
    }

    @media (max-width: 320px) {
        .image-1 {
            height: 160px;
        }
    }
</style>
