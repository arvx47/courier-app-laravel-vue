<script>
import { Doughnut } from 'vue-chartjs';

export default {
	extends: Doughnut,
	// eslint-disable-next-line vue/require-prop-types
	props: ['height'],
	mounted () {
		this.renderChart({
			labels: ['VueJs', 'EmberJs', 'ReactJs', 'AngularJs'],
			datasets: [
				{
					backgroundColor: [
						'#41B883',
						'#E46651',
						'#00D8FF',
						'#DD1B16'
					],
					data: [40, 20, 80, 10]
				}
			]
		}, {responsive: true, maintainAspectRatio: false});
	}
};
</script>
