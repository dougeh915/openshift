This is the openshift project directory

Local commands to run from within the directory are:

The prereq check is:

ansible-playbook -i inventory ./openshift-ansible/playbooks/prerequisites.yml

The real cluster is going to be formed by:

ansible-playbook -i inventory ./openshift-ansible/playbooks/deploy_cluster.yml

To tear down the cluster,

ansible-playbook -i inventory ./openshift-ansible/playbooks/adhoc/uninstall.yml
