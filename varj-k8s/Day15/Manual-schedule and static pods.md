post entering into the container 
cat <<EOF > /etc/kubernetes/manifests/static-pod.yaml
apiVersion: v1
kind: Pod
metadata:
  name: nginx-static-pod
spec:
  containers:
    - name: nginx-container
      image: nginx
      ports:
        - containerPort: 80
EOF
create the static pod using this