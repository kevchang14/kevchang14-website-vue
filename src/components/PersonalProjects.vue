<template>
  <b-container>
    <div class="text-center row">
      <div class="col-sm-12">
        <h1>
          Personal Projects
        </h1>
      </div>
    </div>
    <div class="row mt-3" v-for="(project, index) in projectList" :key="index">
      <div class="col-md-3">
        <h2>
          {{project.title}}
        </h2>
      </div>
      <div class="col-md-9">
        {{project.description}}  
      </div>
    </div>
  </b-container>
</template>

<script>
export default {
  name: 'PersonalProjects',
  /*props: {
    list: Array,
  }*/
  data: function() {
    return {
      projectList: [
        { 
          title: 'Personal Website', 
          description: 'You\'re currently looking at it! Learned Vue to experience a new front end framework and \
          implemented a CI pipeline from GitHub through S3. Static content is deployed from a S3 bucket through the \
          CloudFront CDN.' 
        },
        { 
          title: 'Real Estate Analytics', 
          description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed mattis auctor porttitor. \
          Donec imperdiet ornare sem, id egestas urna molestie at. Vivamus sit amet nisi ut sem euismod consectetur. \
          Aenean non imperdiet diam. Sed eget enim quis mi suscipit auctor in id mi. Cras finibus efficitur nisl id \
          dictum. Aenean imperdiet lectus vitae tristique dictum. Phasellus ultricies felis ut dictum efficitur. \
          Donec sed libero quis sapien vehicula viverra. Donec luctus convallis aliquam. Ut non lectus dignissim, \
          lacinia justo eget, porttitor massa. Nam ac rutrum justo. Pellentesque molestie dui vitae varius maximus. \
          Proin mollis pellentesque porttitor. Orci varius natoque penatibus et magnis dis parturient montes, \
          nascetur ridiculus mus. In aliquam mollis dapibus.' 
        },
      ]
    }
  }
}
</script>