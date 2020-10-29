<template>
  <div class="container mt-5">
    <div v-if="error.statusCode === 403" class="page-error">
      <div class="page-inner">
        <h1>403</h1>
        <div class="page-description">You do not have access to this page.</div>
        <div class="page-search">
          <form>
            <div class="form-group floating-addon floating-addon-not-append">
              <div class="input-group">
                <div class="input-group-prepend">
                  <div class="input-group-text">
                    <i class="fas fa-search"></i>
                  </div>
                </div>
                <input type="text" class="form-control" placeholder="Search" />
                <div class="input-group-append">
                  <button class="btn btn-primary btn-lg">Search</button>
                </div>
              </div>
            </div>
          </form>
          <div class="mt-3">
            <nuxt-link to="/dashboard/ecommerce">Back to Home</nuxt-link>
          </div>
        </div>
      </div>
    </div>
    <div v-if="error.statusCode === 404" class="page-error">
      <div class="page-inner">
        <h1>404</h1>
        <div class="page-description">The page you were looking for could not be found.</div>
        <div class="page-search">
          <form>
            <div class="form-group floating-addon floating-addon-not-append">
              <div class="input-group">
                <div class="input-group-prepend">
                  <div class="input-group-text">
                    <i class="fas fa-search"></i>
                  </div>
                </div>
                <input type="text" class="form-control" placeholder="Search" />
                <div class="input-group-append">
                  <button class="btn btn-primary btn-lg">Search</button>
                </div>
              </div>
            </div>
          </form>
          <div class="mt-3">
            <nuxt-link to="/dashboard/ecommerce">Back to Home</nuxt-link>
          </div>
        </div>
      </div>
    </div>
    <div v-if="error.statusCode === 500" class="page-error">
      <div class="page-inner">
        <h1>500</h1>
        <div class="page-description">Whoopps, something went wrong.</div>
        <div class="page-search">
          <form>
            <div class="form-group floating-addon floating-addon-not-append">
              <div class="input-group">
                <div class="input-group-prepend">
                  <div class="input-group-text">
                    <i class="fas fa-search"></i>
                  </div>
                </div>
                <input type="text" class="form-control" placeholder="Search" />
                <div class="input-group-append">
                  <button class="btn btn-primary btn-lg">Search</button>
                </div>
              </div>
            </div>
          </form>
          <div class="mt-3">
            <nuxt-link to="/dashboard/ecommerce">Back to Home</nuxt-link>
          </div>
        </div>
      </div>
    </div>
    <div v-if="error.statusCode === 503" class="page-error">
      <div class="page-inner">
        <h1>503</h1>
        <div class="page-description">Be right back.</div>
        <div class="page-search">
          <form>
            <div class="form-group floating-addon floating-addon-not-append">
              <div class="input-group">
                <div class="input-group-prepend">
                  <div class="input-group-text">
                    <i class="fas fa-search"></i>
                  </div>
                </div>
                <input type="text" class="form-control" placeholder="Search" />
                <div class="input-group-append">
                  <button class="btn btn-primary btn-lg">Search</button>
                </div>
              </div>
            </div>
          </form>
          <div class="mt-3">
            <nuxt-link to="/dashboard/ecommerce">Back to Home</nuxt-link>
          </div>
        </div>
      </div>
    </div>
    <div class="simple-footer mt-5">Copyright &copy; Nuxt Stisla 2020</div>
  </div>
</template>

<script>
export default {
  props: ["error"],
  layout: "defaultBlank",
};
</script>